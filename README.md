# 🌿 Smart Greenhouse Management System

An Arduino-based automation system that monitors **temperature**, **humidity**, **soil moisture**, and **light intensity**, and automatically controls irrigation.

## 📦 Features

- 🌡 Monitors temperature (DHT22)
- 💧 Tracks humidity levels
- 🌱 Detects soil moisture (analog sensor)
- ☀️ Reads light intensity
- 🚰 Auto-controls irrigation based on soil dryness

## 🔌 Hardware Requirements

| Component              | Arduino Pin |
|------------------------|-------------|
| DHT22 Sensor (Data)    | D2          |
| Soil Moisture Sensor   | A0          |
| Light Sensor / Potentiometer | A4     |
| Relay Module (IN)      | D3          |

## ⚙️ How It Works

- If **soil moisture < 40%**, the **irrigation system (relay)** is turned ON.
- If **soil moisture ≥ 40%**, the irrigation is turned OFF.
- Data is printed to the Serial Monitor every 2 seconds.

## 🧑‍💻 Setup Instructions

1. Open `sketch.ino` in Arduino IDE
2. Install the **DHT sensor library** from the Library Manager
3. Connect your components according to the pin table above
4. Upload the code
5. Open Serial Monitor (baud: 9600)

## 🧪 Simulation

Use [Wokwi](https://wokwi.com) to simulate:
- Light sensor with a potentiometer
- Observe serial output & irrigation behavior

## 📜 License

MIT License
