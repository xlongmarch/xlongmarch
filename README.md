# Hey, I'm xlongmarch 👋

Mobile repair technician | Arduino coder | Crypto enthusiast | Turf accountant  
I love tinkering with hardware, coding projects, and exploring tech.

## Featured Project: 5 Red LED Blink (Arduino)
A simple Arduino project that blinks 5 red LEDs one by one.

##Hardware
5 Red LEDs
5 Resistors (220-330 ohms)
Arduino board
Breadboard & wires
Connect LEDs to pins 2-6, with cathodes to GND via resistors. Upload the code and enjoy the blink!


### Code
```cpp
// Define the LED pins
const int led1 = 2;  // LED 1 connected to pin 2
const int led2 = 3;  // LED 2 connected to pin 3
const int led3 = 4;  // LED 3 connected to pin 4
const int led4 = 5;  // LED 4 connected to pin 5
const int led5 = 6;  // LED 5 connected to pin 6

const int delayTime = 500;  // 500ms = 0.5 seconds

void setup() {
  pinMode(led1, OUTPUT);
  pinMode(led2, OUTPUT);
  pinMode(led3, OUTPUT);
  pinMode(led4, OUTPUT);
  pinMode(led5, OUTPUT);
  digitalWrite(led1, LOW);
  digitalWrite(led2, LOW);
  digitalWrite(led3, LOW);
  digitalWrite(led4, LOW);
  digitalWrite(led5, LOW);
}

void loop() {
  digitalWrite(led1, HIGH);
  delay(delayTime);
  digitalWrite(led1, LOW);
  digitalWrite(led2, HIGH);
  delay(delayTime);
  digitalWrite(led2, LOW);
  digitalWrite(led3, HIGH);
  delay(delayTime);
  digitalWrite(led3, LOW);
  digitalWrite(led4, HIGH);
  delay(delayTime);
  digitalWrite(led4, LOW);
  digitalWrite(led5, HIGH);
  delay(delayTime);
  digitalWrite(led5, LOW);
}



