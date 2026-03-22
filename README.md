# arduino-traffic-simulator
Traffic light system using Arduino
# 🚦 Traffic Light System using Arduino

## 📌 Description
This project simulates a real traffic signal using Arduino.

## 🧰 Components Used
- Arduino Uno
- 3 LEDs (Red, Yellow, Green)
- Resistors
- Breadboard

## ⚙️ Working
- Red LED → Stop (5 sec)
- Green LED → Go (5 sec)
- Yellow LED → Wait (2 sec)

## 💻 Code
Uploaded in this repository.

## 👨‍💻 Author
Parv Jain
int red = 13;
int yellow = 12;
int green = 11;

void setup() {
  pinMode(red, OUTPUT);
  pinMode(yellow, OUTPUT);
  pinMode(green, OUTPUT);
}

void loop() {
  // RED ON
  digitalWrite(red, HIGH);
  digitalWrite(yellow, LOW);
  digitalWrite(green, LOW);
  delay(5000); // 5 seconds

  // GREEN ON
  digitalWrite(red, LOW);
  digitalWrite(yellow, LOW);
  digitalWrite(green, HIGH);
  delay(5000);

  // YELLOW ON
  digitalWrite(red, LOW);
  digitalWrite(yellow, HIGH);
  digitalWrite(green, LOW);
  delay(2000); // 2 seconds
}
