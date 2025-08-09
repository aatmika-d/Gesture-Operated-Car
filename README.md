# Gesture-Controlled Car using Arduino and Accelerometer

## Overview
This project presents a hand-gesture-controlled car system using an Arduino Uno, L293D Motor Driver, RF Module, and ADXL335 Accelerometer. The accelerometer captures 3-axis hand movements, which are wirelessly transmitted via an RF module to the Arduino on the car. The received data is processed to recognize gestures that control the car's movements intuitively.

## Features
- Wireless transmission of gesture data using RF modules
- Real-time hand gesture recognition using accelerometer data
- Motor control with L293D driver for forward, backward, left, and right movement
- Achieved approximately 80% accuracy in gesture recognition

## Hardware Components
- Arduino Uno (Transmitter and Receiver)
- ADXL335 3-axis Accelerometer
- L293D Motor Driver IC
- RF Transmitter and Receiver modules (e.g., REES52)
- DC Motors and Car chassis

## Software
- Arduino IDE for programming Arduino Uno
- Gesture recognition algorithm implemented on Arduino for interpreting accelerometer data

## Getting Started

### Running the Code
The code is written in **Arduino C++** and must be uploaded to the Arduino boards using the **Arduino IDE**.

- Rename your code file(s) with the `.ino` extension (not `.txt`).
- Open the `.ino` files in Arduino IDE.
- Connect your Arduino Uno via USB.
- Select the correct board and COM port under **Tools**.
- Upload the code separately to the Transmitter and Receiver units.

### File Organization
- `Transmitter.ino` — Code for the gesture capturing unit (accelerometer + Arduino + RF transmitter)
- `Receiver.ino` — Code for the car control unit (Arduino + RF receiver + motor driver)

## How It Works
1. The ADXL335 accelerometer captures hand motion data on three axes.
2. Arduino processes the analog data and sends it wirelessly through the RF transmitter.
3. The receiver Arduino receives the data and interprets it using the gesture recognition algorithm.
4. Based on recognized gestures, the L293D motor driver controls the motors to move the car accordingly.
