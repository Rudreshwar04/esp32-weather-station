# ESP32 Weather Station

IoT weather monitor built with ESP32 and DHT22. Displays live readings on an OLED and uploads data to ThingSpeak over Wi-Fi.

## Features
- Temperature and humidity sensing
- Live display on 0.96" OLED (I2C)
- Cloud upload every 30 seconds
- Wi-Fi auto-reconnect

## Components
| Component | Qty |
|---|---|
| ESP32 DevKit V1 | 1 |
| DHT22 sensor | 1 |
| SSD1306 OLED (I2C) | 1 |
| Breadboard + jumper wires | - |

## Circuit
| Device | Pin | ESP32 Pin |
|---|---|---|
| DHT22 | Data | GPIO 4 |
| OLED | SDA | GPIO 21 |
| OLED | SCL | GPIO 22 |

## Setup
1. Install Arduino IDE + ESP32 board package
2. Install libraries: DHT sensor library, Adafruit SSD1306, Adafruit GFX
3. Add your Wi-Fi and ThingSpeak API key in `config.h`
4. Upload `weather_station.ino`

## Future Improvements
- Add BMP280 for pressure
- Battery + deep sleep mode
- Mobile dashboard

## Author
Rudreshwar, ECE, SRMIST

## License
MIT