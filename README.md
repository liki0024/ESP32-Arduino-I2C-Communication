# ESP32-Arduino I²C Communication

An embedded communication project demonstrating I²C communication between an ESP32 and an Arduino, with a Wi-Fi-based web interface on the ESP32.

## Project Overview

This project demonstrates communication between an ESP32 and an Arduino using the I²C protocol.

The Arduino is configured as an I²C slave with address `0x04`, while the ESP32 communicates with the Arduino over the I²C bus.

The ESP32 also uses Wi-Fi and a web interface to provide interaction with the embedded system.

## System Architecture

```text
                 Wi-Fi
                   │
                   ▼
            ┌─────────────┐
            │    ESP32    │
            │ Web Server  │
            └──────┬──────┘
                   │
                  I²C
                   │
                   ▼
            ┌─────────────┐
            │   Arduino   │
            │ I²C Slave   │
            │ Address 0x04 │
            └─────────────┘
