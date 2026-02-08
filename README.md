# Sensor Sound System (SSS)

A discreet sensor-triggered ambience machine designed for a mini-fridge or bar setup. The system detects activity (such as door) and plays randomized sound effects after a number of occurrences. System also doubles as a small standalone speaker system.

## Goal

Create a low-cost, compact device that:

- Detects doors open/close events using a hall effect sensor
- Plays short sound effects or ambience audio
- Randomizes playback timing
- Blends into the environment (hidden / discreet)
- ~$40 budget build

## Features (Planned)

- Sensor-triggered audio playback
- Randomized trigger count before sound plays
- Custom sound files (user selectable)
- Stereo speaker output
- Small enclosure for hidden placement
- Optional Bluetooth / IoT control (future)

## BOM

https://docs.google.com/spreadsheets/d/1TtEXAzZh78ohhP923dgVh_xGt424K24asCBcOYmhk0M/edit?usp=sharing

## System Architecture

**Subsystems:**

- Power Distribuition Board (PDB)
- Control Unit (MCU)
- Sensors (Hall EFfec)
- Audio Module (DAC)
- Speakes

**Block Flow:**

Sensor → MCU → Audio Storage → DAC/Amp → Speakers

Power → All subsystems

## Candidate Microcontrollers

- ESP32
- Arduino Nano 33 IoT
- Raspberry Pi Pico W

Selection will depend on cost, available peripherals, and audio support.

## Exploratory Sensor Options

- Vibration sensor (detect fridge movement)
- Reed switch (door open/close)
- Small accelerometer module
- PIR motion sensor (area detection)

## Audio Module Options

- I2S DAC + small class-D amp
- All-in-one audio playback module
- MCU PWM + filter + amp (low cost option)

## Constraints

- Target budget: $40
- Small and discreet
- Hidden system that blends well

## Status

Concept and architecture defined.  
Parts selection in progress.
**Budget pending, BOM in progress**
