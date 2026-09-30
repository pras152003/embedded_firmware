# embedded_firmware
                   ┌─────────────────────┐
                   │     Linux PC        │
                   │                     │
                   │ Python Test Engine  │
                   │ Shell Scripts       │
                   │ Log Analyzer        │
                   │ Test Reports        │
                   └──────────┬──────────┘
                              │
                         UART / USB
                              │
                              ▼
                   ┌─────────────────────┐
                   │   MCU / ESP32       │
                   │                     │
                   │ Firmware            │
                   │ Sensor Interface    │
                   │ UART                │
                   │ SPI / I2C           │
                   │ CRC                  │
                   │ Watchdog            │
                   └──────────┬──────────┘
                              │
                              ▼
                   ┌─────────────────────┐
                   │ Radar Data Simulator│
                   │ / Sensor            │
                   └─────────────────────┘
# layer1 embedded firmware

ESP32
  ↓
C
  ↓
UART/I2C/SPI
  ↓
Sensor interface

# layer 2 linux

Linux
 ↓
Shell
 ↓
Device communication
 ↓
Logs
 ↓
Process management

# layer 3 automation
Python
 ↓
pytest
 ↓
Test cases
 ↓
Fault injection
 ↓
Logs
 ↓
Report



# phase 1
# Phase 1 — C + Embedded C
2–3 weeks

C fundamentals
Pointers
Arrays
Strings
Structures
Functions
Memory
Bit manipulation
volatile
static
const
Function pointers
