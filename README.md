# HoverTunIX
Gesture Volume Controller

<img width="341" height="351" alt="image" src="https://github.com/user-attachments/assets/3010d9c0-7c8d-446d-8c41-6ee5fde4fc49" />





# 🎵 HoverTunIX: Gesture Volume Controller

Control your computer's volume and media playback using hand gestures! HoverTune uses an ultrasonic distance sensor to detect hand position and translate it into media controls.

![Python](https://img.shields.io/badge/python-3.7+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)


## 🛠️ Hardware Requirements

- **ToF Sensor** (VL53L1X, or similar)
- <img src="https://github.com/user-attachments/assets/4e2f591d-f660-4d8b-be88-029a937283f6" width="300">
  
- **Nucleo STM32F446RE Microcontroller or Equivalent** (to read sensor and send data via serial)
  
  <img src="https://github.com/user-attachments/assets/efe2926f-fd99-4a7e-8cef-47b519df5092" width="300">

- **USB Cable** for serial connection

## 🔌 Wiring

| VL53L1X | STM32F446RE |
|---------|-------------|
| VIN     | 3.3V        |
| GND     | GND         |
| SDA     | PC12 (I2C2)  |
| SCL     | PB10 (I2C2)  |


## 🛠️ STM32 Firmware Setup

1. Open **STM32CubeMX** → New Project → Select `NUCLEO-F446RE`
2. Enable **I2C2** (100kHz) on PC12/PB10
3. Enable **USART2** (Async, 115200 baud) for USB serial
4. Add [VL53L1X ULD driver] to `Core/Src` and `Core/Inc`

## 💻 Software Requirements

- **Python 3.7+**
- **Windows** (uses Windows media key mappings)

## 🚀 Installation


