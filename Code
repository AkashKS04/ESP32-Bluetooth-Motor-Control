#include "BluetoothSerial.h"

BluetoothSerial SerialBT;

int IN1 = 26;
int IN2 = 27;

void setup() {
  pinMode(IN1, OUTPUT);
  pinMode(IN2, OUTPUT);

  Serial.begin(115200);
  SerialBT.begin("ESP32_MOTOR");

  Serial.println("Bluetooth Motor Control Started");
}

void loop() {
  if (SerialBT.available()) {
    char cmd = SerialBT.read();

    if (cmd == '1') {
      digitalWrite(IN1, HIGH);
      digitalWrite(IN2, LOW);
    }
    else if (cmd == '0') {
      digitalWrite(IN1, LOW);
      digitalWrite(IN2, LOW);
    }
  }
}
