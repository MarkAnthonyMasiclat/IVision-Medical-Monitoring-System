# IVision Medical Monitoring System

**IVision** is a team project that builds a medical monitoring system for IV chambers. The system tracks and regulates liquid flow using microcontroller-based sensing and wireless communication to ensure patient safety.

## Project Overview
The system automates monitoring of IV liquid flow, providing real-time alerts for irregular flow or dislodgement, reducing the need for manual checks by medical staff. It combines hardware sensors, IoT services, and cloud integration to create a reliable and safe monitoring solution.

> **Note:** This repository only contains my contributions (ESP32 sensor programming). The team also worked on other parts of the project.

## My Contributions
- Programmed and calibrated the **ESP32 (XIAO_ESP32S3)** sensors to accurately measure liquid flow.  
- Implemented fail-safe mechanisms using:
  - **Accelerometer** to detect movement or dislodgement  
  - **LED** indicators for visual alerts  
- Flow rate monitoring:
  - System detects if the flow deviates beyond a set threshold and triggers an error  
  - Pauses measurement for 10 seconds if irregularities are detected, then resumes automatically  
- Integrated **RFID** for patient and staff login, sending anonymized IDs to the database via MQTT (GDPR compliant)

## Other Team Contributions
- **Teammate 1:** Built the **IoT infrastructure**, including Node-RED flows, cloud integration via Microsoft Azure, and database setup with PostgreSQL and InfluxDB.  
- **Teammate 2:** Designed the **CAD model for the system casing**, ensuring the hardware fits securely and is safe for medical use.  

## Technologies Used
- **Hardware:** ESP32 XIAO_ESP32S3, RFID, Laser + IR sensor, Accelerometer, LED  
- **Software / Services:** MQTT  
- **Programming:** C/C++ (ESP32 sensors)
