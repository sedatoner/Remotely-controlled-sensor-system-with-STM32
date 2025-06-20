# Remotely-controlled-sensor-system-with-STM32
STM32 mikrodenetleyici ile uzaktan kontrol edilen bir sensör sistemi
# Remotely Controlled Sensor System with STM32

This project demonstrates a simple remote sensor system using STM32F103 and a Bluetooth module (HC-05). The user can send a command over Bluetooth (e.g., from a phone), and the microcontroller responds with sensor data.

## Features

- Remote control via Bluetooth (UART)
- Temperature reading (simulated or via DHT11)
- Command-response architecture

## How It Works

1. Send the string `READ` via Bluetooth.
2. STM32 reads temperature from the sensor.
3. The result is sent back as a string (e.g., `Temperature: 27 C`).

## Hardware

- STM32F103 (Blue Pill)
- HC-05 Bluetooth Module
- DHT11 Temperature/Humidity Sensor (or simulated value)
- 10kΩ pull-up resistor

## UART Settings

- Baud rate: 9600
- Word length: 8 bits
- Stop bits: 1
- No parity

