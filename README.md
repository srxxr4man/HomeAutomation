# ESP32 Smart Home Automation System using Blynk IoT

## Overview

This project is a comprehensive IoT-based Home Automation System developed using the ESP32 microcontroller and the Blynk IoT platform. It provides real-time remote control and monitoring of household devices through a smartphone application while also implementing intelligent automation features.

The system integrates multiple sensors and actuators to create a smart environment capable of controlling lights, monitoring temperature and humidity, automating night lighting, and operating a smart gate system.

---

## Features

### Remote Appliance Control

* Control Living Room Light through the Blynk mobile application.
* Control Bedroom Light through the Blynk mobile application.
* Real-time synchronization between ESP32 and Blynk dashboard.

### Smart Gate Automation

* Manual gate control using the Blynk application.
* Automatic gate operation using an IR sensor for object detection.
* Servo motor-based gate mechanism.

### Environmental Monitoring

* Real-time temperature monitoring using DHT11 sensor.
* Real-time humidity monitoring using DHT11 sensor.
* Live sensor data displayed on the Blynk dashboard.

### Intelligent Night Light

* Automatic night light control using an LDR sensor.
* Turns ON during low-light conditions.
* Turns OFF during daylight conditions.
* Displays current night light status in the Blynk app.

---

## Hardware Components

| Component                           | Quantity    |
| ----------------------------------- | ----------- |
| ESP32 Development Board             | 1           |
| DHT11 Temperature & Humidity Sensor | 1           |
| LDR Sensor                          | 1           |
| IR Obstacle Detection Sensor        | 1           |
| Servo Motor (SG90/MG90S)            | 1           |
| Relay Module                        | 2           |
| LEDs / Bulbs                        | 2           |
| Jumper Wires                        | As Required |
| Breadboard                          | 1           |

---

## Pin Configuration

| Component         | ESP32 Pin |
| ----------------- | --------- |
| Living Room Relay | GPIO 26   |
| Bedroom Relay     | GPIO 27   |
| Night Light       | GPIO 19   |
| LDR Sensor        | GPIO 34   |
| IR Sensor         | GPIO 14   |
| DHT11 Sensor      | GPIO 4    |
| Servo Motor       | GPIO 13   |

---

## Blynk Virtual Pins

| Virtual Pin | Function                     |
| ----------- | ---------------------------- |
| V0          | Living Room Light Control    |
| V1          | Bedroom Light Control        |
| V2          | Manual Gate Control          |
| V3          | Temperature Display          |
| V4          | Humidity Display             |
| V5          | Night Light Status Indicator |
| V6          | Night Light Text Status      |

---

## Working Principle

1. The ESP32 connects to Wi-Fi and the Blynk Cloud.
2. Users can remotely control lights using the Blynk application.
3. Temperature and humidity data are continuously collected from the DHT11 sensor and sent to the dashboard.
4. The LDR sensor monitors ambient light levels and automatically controls the night light.
5. The IR sensor detects approaching objects and automatically opens the gate using a servo motor.
6. Users can also manually operate the gate through the Blynk interface.

---

## Technologies Used

* ESP32
* Arduino IDE
* Blynk IoT Platform
* C++
* Embedded Systems
* IoT Automation

---

## Future Improvements

* Voice Assistant Integration (Google Assistant/Alexa)
* Energy Consumption Monitoring
* Mobile Push Notifications
* Smart Scheduling for Appliances
* MQTT Integration
* Camera-based Security Monitoring

---

## Project Demonstration

Add project photos, circuit diagrams, and demonstration videos here.

Example:

/images
├── circuit_diagram.png
├── hardware_setup.jpg
├── blynk_dashboard.png

---

## Author

**A Sreeram, Asil Sameer, Yadav Baiju and Astin Shibu**

Aritificial Intelligence and Data Science Engineering Student

Passionate about IoT, Embedded Systems, Automation, and Smart Technologies.

---
