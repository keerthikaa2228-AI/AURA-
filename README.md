# AURA

AURA is a jewelry-like wearable research prototype for physiological and motion sensing, signal-quality analysis, and experimental ML.

## Concept

AURA is designed as a compact wearable pendant paired with a mobile application.

The system explores:

- Optical physiological sensing
- Motion sensing
- Signal-quality assessment
- Data collection and visualization
- Experimental ML analysis
- A future compact custom PCB
- A 3D-printed pendant enclosure

## AURA Concept

### Exterior Design

![AURA exterior design](AURA%20design%20outer)

### Internal Electronics Concept

![AURA internal electronics](AURA%20pendant%20circuit%20inner)

### Companion App

![AURA app UI](AURA%20app%20UI)

## Current Prototype Architecture

```text
MAX30102 PPG ──┐
               ├── I2C ── ESP32 DevKit v1
MPU6050 IMU ───┘
                         │
                         ├── Signal quality
                         ├── Preprocessing
                         └── BLE
                              │
                              ↓
                          AURA App
.
