//paste this into Arduino IDE and upload to your Arduino!

#include <Servo.h>

Servo servo_9;

// Helper function to set pins 2 through 8 quickly
void setPins(int d2, int d3, int d4, int d5, int d6, int d7, int d8) {
  digitalWrite(2, d2);
  digitalWrite(3, d3);
  digitalWrite(4, d4);
  digitalWrite(5, d5);
  digitalWrite(6, d6);
  digitalWrite(7, d7);
  digitalWrite(8, d8);
}

// Helper function to turn off all output pins
void clearPins() {
  setPins(LOW, LOW, LOW, LOW, LOW, LOW, LOW);
}

void setup() {
  servo_9.attach(9, 500, 2500);
  
  // Set pins 2 to 8 as outputs using a loop
  for (int i = 2; i <= 8; i++) {
    pinMode(i, OUTPUT);
  }
}

void loop() {
  servo_9.write(0);

  // Sequence step 1
  setPins(HIGH, HIGH, HIGH, HIGH, HIGH, HIGH, LOW);
  delay(1000);
  clearPins();
  delay(1000);

  // Sequence step 2
  setPins(LOW, HIGH, HIGH, LOW, LOW, LOW, LOW);
  delay(1000);
  clearPins();
  delay(1000);

  // Sequence step 3
  setPins(HIGH, HIGH, LOW, HIGH, HIGH, LOW, HIGH);
  delay(1000);
  clearPins();
  delay(1000);

  // Sequence step 4
  setPins(HIGH, HIGH, HIGH, HIGH, LOW, LOW, HIGH);
  delay(1000);
  clearPins();
  delay(1000);

  // Sequence step 5
  setPins(LOW, HIGH, HIGH, LOW, LOW, HIGH, HIGH);
  delay(1000);
  clearPins();
  delay(1000);

  // Sequence step 6
  setPins(HIGH, LOW, HIGH, HIGH, LOW, HIGH, HIGH);
  delay(1000);
  clearPins();
  delay(1000);

  // Sequence step 7
  setPins(HIGH, LOW, HIGH, HIGH, HIGH, HIGH, HIGH);
  delay(1000);
  clearPins();
  delay(1000);

  // Sequence step 8
  setPins(HIGH, HIGH, HIGH, LOW, LOW, LOW, LOW);
  delay(1000);
  clearPins();
  delay(1000);

  // Sequence step 9
  setPins(HIGH, HIGH, HIGH, HIGH, HIGH, HIGH, HIGH);
  delay(1000);
  clearPins();
  delay(1000);

  // Sequence step 10
  setPins(HIGH, HIGH, HIGH, HIGH, LOW, HIGH, HIGH);
  delay(1000);
  clearPins();
  delay(1000);

  // Final servo actions
  servo_9.write(0);
  delay(1000);
  servo_9.write(180);
  delay(1000);
}
