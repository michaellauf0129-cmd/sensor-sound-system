# Sensor Sound System

A discreet sensor-triggered ambience machine designed for a mini-fridge or bar setup. The system detects activity (such as door open, vibration, or motion) and plays randomized sound effects after a configurable number of trigger events. It can also function as a small standalone speaker system.

## Goal

Create a low-cost, compact device that:

- Detects fridge or bar interaction using a sensor
- Plays short sound effects or ambience audio
- Randomizes playback timing after multiple events
- Blends into the environment (hidden / discreet)
- Stays under a ~$20 build budget

## Features (Planned)

- Sensor-triggered audio playback
- Randomized trigger count before sound plays
- Custom sound files (user selectable)
- Stereo speaker output
- Small enclosure for hidden placement
- Optional Bluetooth / IoT control (future)

## System Architecture

**Subsystems:**

- Power supply (battery or wall adapter)
- Sensor input (vibration, motion, or door switch)
- Microcontroller (processing + control logic)
- Audio storage (flash or SD card)
- Audio DAC / amplifier module
- Left and right speakers

**Block Flow:**

Sensor → MCU → Audio Storage → DAC/Amp → Speakers

Power → All subsystems

## Candidate Microcontrollers

- ESP32
- Arduino Nano 33 IoT
- Raspberry Pi Pico W

Selection will depend on cost, available peripherals, and audio support.

## Sensor Options

- Vibration sensor (detect fridge movement)
- Reed switch (door open/close)
- Small accelerometer module
- PIR motion sensor (area detection)

## Audio Options

- I2S DAC + small class-D amp
- All-in-one audio playback module
- MCU PWM + filter + amp (low cost option)

## Operation Logic (Planned)

- Monitor sensor input
- Count trigger events
- When count reaches randomized threshold:
  - Select random audio clip
  - Play sound
  - Reset counter with new random threshold

## Constraints

- Target budget: $20
- Small form factor
- Simple wiring
- Beginner-friendly firmware

## Status

Concept and architecture defined.  
Parts selection and firmware implementation in progress.
