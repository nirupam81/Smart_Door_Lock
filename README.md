🚪 Smart Door Lock System
An IoT-based security solution designed to automate door access using microcontrollers. This project integrates hardware and software to provide a secure, convenient, and keyless entry system.

📖 Table of Contents
Overview

Features

Hardware Requirements

Software & Libraries

Circuit Diagram

Installation

How It Works

Future Enhancements

🔍 Overview
The Smart Door Lock is a prototype designed to replace traditional mechanical keys with digital authentication. It uses a microcontroller to process signals from authentication modules (Bluetooth/RFID/Keypad) and actuates a servo motor to lock or unlock the door.

✨ Features
Keyless Entry: Unlock your door via a Smartphone App (Bluetooth/Wi-Fi).

Multiple Auth Methods: Supports RFID tags and physical Keypads.

Real-time Feedback: Integrated LEDs and Buzzers for status alerts.

Auto-Lock: Automatically secures the door after a set duration.

Low Power Consumption: Optimized for battery-operated performance.

🛠 Hardware Requirements
To build this project, you will need:

Microcontroller: Arduino Uno, Nano, or NodeMCU (ESP8266).

Actuator: MG995 or SG90 Servo Motor.

Bluetooth Module: HC-05 or HC-06 (for wireless control).

RFID Module: RC522 (optional).

Others: 16x2 I2C LCD Display, 4x4 Matrix Keypad, Buzzer, Jumper Wires.

💻 Software & Libraries
The following tools and libraries were used:

Arduino IDE

Libraries:

Servo.h - For motor control.

SoftwareSerial.h - For Bluetooth communication.

SPI.h & MFRC522.h - For RFID functionality.

LiquidCrystal_I2C.h - For the display interface.

⚡ Installation
Clone the Repository:

Bash
git clone https://github.com/nirupam81/Smart_Door_Lock.git
Hardware Setup: Connect the components according to the circuit diagram provided in the /docs folder.

Upload Code:

Open Smart_Door_Lock.ino in the Arduino IDE.

Select your board and port.

Click Upload.

Mobile App: (If applicable) Install the .apk file located in the /app folder.

⚙️ How It Works
The system stays in a "Listening" state.

The user provides input via the Mobile App or an RFID tag.

The microcontroller verifies the data:

If Authorized: The Servo rotates (e.g., 90°) to unlock.

If Unauthorized: Access is denied, and the buzzer sounds.

The LCD displays the current status (Locked/Unlocked).

🚀 Future Enhancements
Fingerprint Sensor: Adding biometric security.

Face Recognition: Using an ESP32-CAM for AI-based entry.

Cloud Integration: Use Blynk or AWS IoT for remote access from anywhere in the world.

OTP System: Temporary passwords for guests.

🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

📜 License
This project is licensed under the MIT License - see the LICENSE file for details.



