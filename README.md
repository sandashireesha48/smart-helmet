# smart-helmet
# Smart Helmet System

## Project Description
An Intelligent IoT-enabled Smart Helmet System designed to improve two-wheeler rider safety and automate accident detection. The system ensures the rider is wearing the helmet, checks for alcohol consumption before starting the vehicle, detects collisions, and sends real-time location alerts in emergencies.

## 🛠️ Hardware Components Used
* **Arduino Uno / Microcontroller** — The central control unit for managing sensor data.
* **MQ-3 Alcohol Sensor** — Detects breath alcohol levels to prevent drunk driving.
* **Ultrasonic Distance Sensor / IR Sensor** — Ensures the helmet is actually being worn by the rider.
* **Vibration / MPU6050 Accelerometer Sensor** — Detects sudden impacts or crash conditions.
* **NEO-6M GPS Module** — Captures coordinates (Latitude & Longitude) during an accident.
* **Wi-Fi Module (ESP8266 / ESP32)** — Handles wireless cloud tracking and emergency messaging.
* **Relay Module** — Controls the vehicle's ignition circuit based on safety checks.

## 💻 Software & Tools
* **Arduino IDE** — Used for writing, compiling, and flashing the firmware.
* **Embedded C++** — Programming language utilized for sensor integration and threshold logic.

## 📌 Main Features & Logic
1. **Ignition Interlocking:** The vehicle relay stays OFF until the ultrasonic sensor confirms the helmet is on and the MQ-3 sensor detects zero alcohol.
2. **Accident Detection:** If the vibration sensor thresholds are crossed, an emergency protocol triggers.
3. **Location Alerting:** The GPS module pulls live coordinates and uploads them via the Wi-Fi/cellular network to notify emergency contacts.
4.
