Gesture-Controlled Car using Arduino and Accelerometer
Overview
This project presents a hand-gesture-controlled car system using an Arduino Uno, L293D Motor Driver, RF Module, and ADXL335 Accelerometer. The accelerometer captures 3-axis hand movements, which are wirelessly transmitted via an RF module to the Arduino on the car. The received data is processed to recognize gestures that control the car's movements intuitively.

Features
Wireless transmission of gesture data using RF modules

Real-time hand gesture recognition using accelerometer data

Motor control with L293D driver for forward, backward, left, and right movement

Achieved approximately 80% accuracy in gesture recognition

Hardware Components
Arduino Uno (Transmitter and Receiver)

ADXL335 3-axis Accelerometer

L293D Motor Driver IC

RF Transmitter and Receiver modules (e.g., REES52)

DC Motors and Car chassis

Software
Arduino IDE for programming Arduino Uno

Gesture recognition algorithm implemented on Arduino for interpreting accelerometer data

Getting Started
Running the Code
The code is written in Arduino C++ and must be uploaded to the Arduino boards using the Arduino IDE.

Make sure to rename your code file with the extension .ino (not .txt).

Open the .ino file in Arduino IDE.

Connect your Arduino Uno board via USB.

Select the correct board and COM port under Tools in Arduino IDE.

Upload the code to the transmitter and receiver units separately.

File Organization
Transmitter.ino — Code for the gesture capturing unit (accelerometer + Arduino + RF transmitter)

Receiver.ino — Code for the car control unit (Arduino + RF receiver + motor driver)

How It Works
The ADXL335 accelerometer captures hand motion data in three axes.

Arduino processes the analog data and sends it wirelessly through the RF transmitter.

The receiver Arduino gets the data and interprets it using the gesture recognition algorithm.

Based on the recognized gesture, the L293D motor driver controls the motors to move the car accordingly.
