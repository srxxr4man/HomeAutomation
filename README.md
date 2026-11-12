# 🏠 ESP32 Smart Home Automation System using Blynk IoT

<p align="center">
  <img src="https://img.shields.io/badge/Platform-ESP32-blue?style=for-the-badge&logo=espressif" />
  <img src="https://img.shields.io/badge/IoT-Blynk-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Language-C++-orange?style=for-the-badge&logo=cplusplus" />
  <img src="https://img.shields.io/badge/IDE-Arduino%20IDE-00979D?style=for-the-badge&logo=arduino" />
</p>

## 📌 Overview

The **ESP32 Smart Home Automation System** is an IoT-based project developed using the ESP32 microcontroller and the Blynk IoT platform. It enables users to remotely control household appliances and monitor environmental conditions through a smartphone application.

The system integrates sensors and actuators to provide smart home functionality, including remote light control, automatic night lighting, temperature and humidity monitoring, and smart gate automation.

By combining Wi-Fi connectivity, sensor-based automation, and mobile application control, this project demonstrates how IoT technology can make everyday home management more convenient and efficient.

---

## ✨ Features

### 💡 Remote Appliance Control
- Control Living Room Light through the Blynk mobile application.
- Control Bedroom Light remotely.
- Synchronize appliance states with the Blynk dashboard.

### 🚪 Smart Gate Automation
- Manual gate operation through the Blynk application.
- Automatic object detection using an IR sensor.
- Servo motor-based gate opening and closing mechanism.

### 🌡️ Environmental Monitoring
- Real-time temperature monitoring using the DHT11 sensor.
- Real-time humidity monitoring.
- Display sensor readings on the Blynk dashboard.

### 🌙 Intelligent Night Light
- Automatic night light control using an LDR sensor.
- Turns ON under low-light conditions.
- Turns OFF during sufficient daylight.
- Displays night light status through the Blynk application.

---

## 🛠️ Hardware Components

| Component | Quantity |
|---|---:|
| ESP32 Development Board | 1 |
| DHT11 Temperature and Humidity Sensor | 1 |
| LDR Sensor | 1 |
| IR Obstacle Detection Sensor | 1 |
| Servo Motor (SG90/MG90S) | 1 |
| Relay Module | 2 |
| LEDs / Bulbs | 2 |
| Jumper Wires | As Required |
| Breadboard | 1 |

---

## 📍 Pin Configuration

| Component | ESP32 GPIO Pin |
|---|---|
| Living Room Relay | GPIO 26 |
| Bedroom Relay | GPIO 27 |
| Night Light | GPIO 19 |
| LDR Sensor | GPIO 34 |
| IR Sensor | GPIO 14 |
| DHT11 Sensor | GPIO 4 |
| Servo Motor | GPIO 13 |

---

## 📱 Blynk Virtual Pin Configuration

| Virtual Pin | Function |
|---|---|
| V0 | Living Room Light Control |
| V1 | Bedroom Light Control |
| V2 | Manual Gate Control |
| V3 | Temperature Display |
| V4 | Humidity Display |
| V5 | Night Light Status Indicator |
| V6 | Night Light Text Status |

---

## ⚙️ Working Principle

1. **Wi-Fi Connection:** The ESP32 connects to the available Wi-Fi network and establishes communication with the Blynk Cloud.
2. **Remote Appliance Control:** Users control the living room and bedroom lights through the Blynk mobile application.
3. **Environmental Monitoring:** The DHT11 sensor collects temperature and humidity readings and sends the values to the Blynk dashboard.
4. **Automatic Night Lighting:** The LDR continuously monitors ambient light intensity. The ESP32 switches the night light ON or OFF based on the detected light level.
5. **Automatic Gate Operation:** The IR sensor detects approaching objects and triggers the servo motor to operate the gate.
6. **Manual Gate Control:** Users can also operate the gate remotely through the Blynk application.

---

## 🔄 System Workflow

```text
             BLYNK MOBILE APP
                    |
                    | Wi-Fi / Cloud
                    |
               ESP32 BOARD
                    |
       +------------+------------+
       |            |            |
   Appliance     Sensors      Gate System
    Control      Monitoring        |
       |            |              |
   +---+---+    +---+---+       IR Sensor
   |       |    |       |           |
Living  Bedroom DHT11   LDR       Servo
Room    Light    |      |          Motor
Light          Temp.  Night       Gate
               Hum.   Light
```

---

## 💻 Technologies Used

| Technology | Purpose |
|---|---|
| ESP32 | Main microcontroller |
| C++ | Embedded programming |
| Arduino IDE | Code development and uploading |
| Blynk IoT | Remote monitoring and control |
| Wi-Fi | Wireless communication |
| DHT11 | Temperature and humidity sensing |
| LDR | Ambient light detection |
| IR Sensor | Object detection |
| Servo Motor | Gate automation |

---

## 📂 Project Structure

```text
├── HomeAutomation
└── README.md
```

*Note: Update the folder and source-file names to match your actual GitHub repository.*

---

## 🚀 Getting Started

### Prerequisites
- Arduino IDE installed.
- ESP32 board package configured in Arduino IDE.
- Blynk account and mobile application.
- Required sensors and hardware components.
- Wi-Fi connection.

### Required Libraries
Install the following libraries through the Arduino IDE Library Manager:

- `Blynk`
- `DHT sensor library`
- `ESP32Servo`

### Setup Instructions

1. Clone or download this repository.
2. Open the project `.ino` file in Arduino IDE.
3. Install the required libraries.
4. Configure the ESP32 board and select the appropriate COM port.
5. Create a Blynk template and configure the required virtual pins.
6. Update the Wi-Fi credentials and Blynk authentication details in the source code.
7. Connect the hardware components according to the pin configuration.
8. Upload the code to the ESP32.
9. Open the Blynk mobile application and test the automation features.

---

## 🔮 Future Improvements

- 🎙️ Voice assistant integration using Google Assistant or Alexa.
- ⚡ Energy consumption monitoring.
- 📲 Mobile push notifications for important events.
- ⏰ Smart scheduling for household appliances.
- 🌐 MQTT protocol integration.
- 📷 Camera-based security monitoring.

---

## 🎓 Academic Details

| Detail | Information |
|---|---|
| Institution | Muthoot Institute of Technology and Science (MITS) |
| Department | Artificial Intelligence and Data Science |
| Project Type | IoT / Embedded Systems |
| Academic Batch | 2025–2029 |
| Semester | Semester 2 |

---

## 👨‍💻 Authors

This project was developed collaboratively by:

- **A Sreeram**
- **Asil Sameer**
- **Yadav Baiju**
- **Astin Shibu**

*Artificial Intelligence and Data Science Engineering Students*

Interested in IoT, Embedded Systems, Automation, and Smart Technologies.

---

<p align="center">
  <b>🏠 Making Homes Smarter with IoT Technology!</b>
</p>
