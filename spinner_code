#include <math.h>

const int buttonPin = 7;
const int ledPair1 = 3;
const int ledPair2 = 4;
const int ledPair3 = 5;
const int ledPair4 = 6;
const int ledPair5 = 7;
const int ledPair6 = 8;
const int ledPair7 = 9;
const int ledPair8 = 10;

int buttonState;

long randomNum;
int numPins = 4;
int currentPin = 0;

int ledArray[8] = {ledPair1, ledPair2, ledPair3, ledPair4,
  ledPair5, ledPair6, ledPair7, ledPair8};

void setup() {
  // put your setup code here, to run once:
  // designated pin for each (or every two) led ouput
  // designated pin for button input


  pinMode(ledPair1, OUTPUT);
  pinMode(ledPair2, OUTPUT);
  pinMode(ledPair3, OUTPUT);
  pinMode(ledPair4, OUTPUT);
  pinMode(ledPair5, OUTPUT);
  pinMode(ledPair6, OUTPUT);
  pinMode(ledPair7, OUTPUT);
  pinMode(ledPair8, OUTPUT);
  pinMode(buttonPin, INPUT);
  Serial.begin(9600);

}
void loop() {
  // put your main code here, to run repeatedly:
  // upon button push cycles through LED pairs, starting fast 
        //and slowing until it lands on one pair and blinks
    buttonState = digitalRead(buttonPin);
    Serial.println(buttonState);
    if (buttonState == HIGH) {
    // start circling lights
      for (int i = 0; i < random(50, 100); i++){
        digitalWrite(ledArray[i%numPins], HIGH);
        double di = pow(i,1.5);
        int wait = di;
        delay(wait);
        digitalWrite(ledArray[i%numPins], LOW);
        delay(100);
        currentPin = i % numPins;
        }
      for (int n = 0; n < 3; n++){
      digitalWrite(ledArray[currentPin], HIGH);
      delay(100);
      digitalWrite(ledArray[currentPin], LOW);
      delay(100);
}
  // cycles through patterns while waiting for button push
}
delay(200);
}
