# ESP32-Battery-Sensor-Board
ESP32-based Lithium Battery Powered Sensor Board ⚡🔋 Low-power ESP32 dev board with 18650 battery, buck regulator, load switch, and sensor interfaces.  Includes KiCad schematic, PCB, Gerber, BOM, and 3D renders for easy fabrication.
# ESP32 Lithium Battery Powered Sensor Board

This repository contains the design files for an **IoT-ready ESP32 development board** powered by a **single-cell lithium battery**.  
The board integrates power management, battery protection, load control, and sensor connectivity, making it ideal for **low-power IoT applications** such as soil moisture monitoring.

---

## 📐 Project Overview
- **MCU:** ESP32-WROOM module (Dev Board footprint)
- **Battery:** Single-cell 18650 Li-ion
- **Power Regulation:** TPS62740 buck regulator (high efficiency, low power)
- **Load Switch:** TPS22918 for peripheral control
- **Protection:** Polyfuse + filtering network
- **Connectivity:**
  - Soil moisture sensor
  - Light sensor
  - External Bluetooth (HC-05 module header)
- **Interfaces:** Multiple GPIO headers for expansion

---

## 📂 Repository Contents
- `Gerber_Assignment.zip` → Gerber files for PCB fabrication
- `ibom.html` → Interactive Bill of Materials (view in browser)
- `Schematic.jpg` → Complete circuit schematic
- `PCB.png` → 2D PCB layout
- `3D_1.png` / `3D_2.png` → 3D renders of the assembled PCB
- `README.md` → Documentation

---

## ⚡ Circuit Features

### 🔋 Battery Connection
- 18650 Li-ion cell holder  
- Polyfuse (resettable fuse) for overcurrent protection  

### 🔌 Buck Regulator (TPS62740)
- Steps down Li-ion voltage (2.5–4.2V) to stable 3.3V  
- Ultra-low quiescent current for energy efficiency  

### 🧠 MCU Section (ESP32 Dev Board)
- Wi-Fi + Bluetooth dual-core microcontroller  
- Powered via `VOUT` from buck regulator  
- Access to GPIO, UART, ADC for sensors  

### 📡 Sensor Connection
- Soil moisture & light sensor headers  
- Powered via regulated 3.3V supply  

### 🔀 Load Switch (TPS22918)
- Controls power to external modules  
- Reduces standby current draw  

### 📶 External Bluetooth
- HC-05 module connector (UART interface)  

---

## 🚀 How to Manufacture
1. Download `Gerber_Assignment.zip`
2. Upload to PCB manufacturer (JLCPCB, PCBWay, etc.)
3. Select:
   - 2 Layer PCB
   - 1.6 mm thickness
   - 1 oz copper
   - HASL finish
4. Place order  

---

## 🛠 Tools Used
- **EDA Tool:** KiCad
- **Microcontroller:** ESP32
- **Designer:** EmbedGyaan – Learn Code & Circuits  

---

## 📜 License
This project is open-source under the **MIT License**.  
Feel free to use, modify, and distribute with attribution.  

---
