# 🤖 ESP32 Autonomous wall following Robot with Mapping & Navigation

An **ESP32-based autonomous robot** designed for **environment mapping, obstacle avoidance, and waypoint-based navigation** using multiple sensors and efficient control algorithms. This project demonstrates **embedded programming**, **sensor fusion**, and **robot navigation** for autonomous applications.

---

## 📌 Features

- **Multi-Sensor Integration**:
  - **VL53L0X ToF Sensors** – for precise distance measurements.
  - **TCS34725 Color Sensor** – for object and surface color detection.
  - **MPU6050 Gyroscope** – for orientation and heading.
- **Motor Control**:
  - N20 DC Motors with encoders for speed and position control.
- **Autonomous Navigation**:
  - Mapping the environment in real-time.
  - Obstacle avoidance algorithms.
  - Waypoint-based navigation.
- **I²C Multiplexing** – handle multiple identical I²C devices without conflicts.
- **Optimized Performance** – replacing `ledcSetup` with an efficient motor control method for reliability.

---

## 📂 Hardware Components

| Component | Description |
|-----------|-------------|
| ESP32 Dev Board | Main controller |
| VL53L0X x3 | Time-of-Flight distance sensors |
| TCS34725 | Color sensor |
| MPU6050 | Gyroscope & accelerometer |
| N20 Motors | 6V, 300 RPM DC motors with encoders |
| TB6612FNG | Dual DC Motor Driver |
| I²C Multiplexer | PCA9548A |
| LiPo Battery | 3S (11.1V) with step-down regulator |
| Chassis | 2-wheel or custom platform |

---

## ⚙️ Software & Libraries

- **Arduino IDE** (with ESP32 board support)
- Libraries:
  - `Wire.h` (I²C communication)
  - `Adafruit_VL53L0X`
  - `Adafruit_TCS34725`
  - `MPU6050`
  - `math.h` and `algorithm` for calculations
- **FreeRTOS** (parallel task execution)

---

## 🚀 Setup Instructions

1. **Install Arduino IDE** and configure ESP32 board support.
2. **Install required libraries**:
   ```bash
   Sketch → Include Library → Manage Libraries
