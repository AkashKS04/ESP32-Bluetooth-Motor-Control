# ESP32 Bluetooth Motor Control 🔵⚙️

This project demonstrates how to control a DC motor using **ESP32 Bluetooth**.
The motor can be turned ON and OFF using a mobile phone via a Bluetooth terminal app.

## 🔧 Components Used
- ESP32 Development Board
- L298N Motor Driver
- DC Motor
- External Power Supply
- Jumper Wires

## 🔌 Connections

### ESP32 → L298N
| ESP32 Pin | L298N Pin |
|---------|-----------|
| GPIO 26 | IN1 |
| GPIO 27 | IN2 |
| GND | GND |

> ⚠️ Make sure ESP32 GND and motor driver GND are common.

### Motor Power
- External battery connected to L298N `+12V` and `GND`

## 📲 Mobile App
Use **Serial Bluetooth Terminal** (Android).

### Commands
- Send `1` → Motor ON
- Send `0` → Motor OFF

## 🧠 How It Works
ESP32 receives Bluetooth commands from the mobile phone and sends control signals
to the L298N motor driver, which safely drives the DC motor.

## 🚀 Future Improvements
- Motor speed control (PWM)
- Direction control
- WiFi-based control
- IoT dashboard

## 📺 YouTube Video
Project explained step-by-step on my YouTube channel:
👉 *link will be added here*

## 🤝 Author
Akash K S  
Embedded Systems & IoT Enthusiast
