#include <Adafruit_Sensor.h>

/*
 1. Go to sketch
 2. Go to Manage Libraries
 3. Install Adafruit unified sensor
 4. Add that Adafruit unified sensor file
 
  
 */

int i = 0;
float temp = 0;
 
void setup() {
  Serial.begin(9600);
}

void loop() {
  i = analogRead(A0); // analog pin A0
  temp = (i/1024.0)*500;
  Serial.println(temp);
  delay(1000);
}
