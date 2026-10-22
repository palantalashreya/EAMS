# ESP32 Firmware

Firmware for acquiring sensor readings from the EAMS hardware prototype.

## Planned Responsibilities

- Initialize sensors
- Read sensor values
- Perform basic signal processing
- Monitor temperature and humidity
- Connect to Wi-Fi
- Send readings to the backend

## Planned Sensors

- MQ-137 — ammonia sensing
- MQ-135 — gas/VOC sensing
- DHT22 — temperature and humidity

## Data Flow

Sensors
↓
ESP32
↓
Sensor Readings
↓
Wi-Fi
↓
Backend API