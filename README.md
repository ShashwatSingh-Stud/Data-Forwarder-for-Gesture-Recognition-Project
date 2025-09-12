# Data-Forwarder-for-Gesture-Recognition-Project
This repository contains the Data Forwarder module designed to support a real-time Gesture Recognition system. It acts as a robust middleware layer that efficiently captures, processes, and transmits gesture data from input devices (e.g., cameras or sensors) to downstream recognition models or visualization interfaces.
MPU6050 Data Forwarder for Gesture Recognition
This is an Arduino sketch designed to forward real-time accelerometer data from an MPU6050 sensor to the Serial Monitor. The data is formatted as a comma-separated values (CSV) stream, making it easy to capture and use for gesture recognition, machine learning, or data analysis projects.

The sketch samples the MPU6050 at a high, configurable frequency (100Hz by default) to ensure smooth and accurate data collection for dynamic movements.

Features
High-Frequency Sampling: Configurable sampling rate for accurate data capture.

CSV Output: Accelerometer data is printed in a clean x,y,z format.

Easy to Use: Simple and clear code for a quick setup.

Prerequisites
An Arduino board (e.g., Uno, Nano, ESP32)

An MPU6050 gyroscope and accelerometer sensor

Jumper wires for connections

Installation and Setup
Hardware Connection:

Connect the MPU6050 to your Arduino board using the I2C protocol.

VCC to Arduino 5V

GND to Arduino GND

SCL to Arduino A5 (or SCL on modern boards)

SDA to Arduino A4 (or SDA on modern boards)

Software Setup:

Open the Arduino IDE.

Go to Sketch -> Include Library -> Manage Libraries...

Search for and install the following libraries:

Adafruit MPU6050

Adafruit Unified Sensor

Upload the Code:

Open the MPU6050_Data_Forwarder.ino file in the Arduino IDE.

Connect your Arduino board to your computer.

Select the correct board and port from the Tools menu.

Click the Upload button to flash the sketch to your board.

Usage
After uploading the sketch, open the Serial Monitor (Tools -> Serial Monitor).

Set the baud rate to 115200.

You will see a continuous stream of accelerometer data in the format
