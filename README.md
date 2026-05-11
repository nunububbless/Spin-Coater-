# Maasi-Inspired ESP32 Spin Coater

A low-cost, open-source spin coater designed for thin-film fabrication and experimental memristor research using an ESP32, brushless motor + ESC system, and a 20x4 LCD button-controlled interface.

Built for:
- paper-based electronics
- low-cost thin-film deposition
- TiO₂ coating experiments
- neuromorphic device fabrication
- student-accessible materials science workflows

---

# Features

- ESP32-based motor control
- Adjustable RPM control
- Adjustable coating duration
- 20x4 LCD interface
- 5-button navigation/control system
- Brushless motor + ESC drive system
- Compact benchtop footprint
- Designed for iterative materials experimentation

---

# User Interface

The system uses a 20x4 LCD display with five physical buttons for navigation and control.

Current controls include:
- Increase RPM
- Decrease RPM
- Increase duration
- Decrease duration
- Start coating cycle

The interface was intentionally designed to remain simple and reliable for laboratory use.

---

# Current Use Case

This system is currently being used for fabrication experiments involving:

- gelatin–salt electrolyte layers
- paper-based ECM memristors
- TiO₂ thin-film deposition
- humidity-sensitive device encapsulation workflows

The spin coater was developed to improve coating uniformity and experimental repeatability in low-cost memristive device fabrication.

---

# Hardware

## Main Components

| Component | Description |
|---|---|
| ESP32 | Main microcontroller |
| 20x4 LCD | User interface display |
| Push Buttons | RPM and timer control |
| ESC | Brushless motor controller |
| FeiChao Brushless Motor | Spin platform drive motor |
| 12V DC Supply | Main power input |

---

# Wiring

## ESC Connections

| ESC Wire | Connection |
|---|---|
| Signal | ESP32 GPIO18 |
| GND | ESP32 GND |
| Power | 12V Supply |

---

# ESC Notes

The ESC requires:
- shared ground with ESP32
- PWM servo-style control
- proper startup arming sequence

A calibration routine is included in the firmware directory.

---

# Firmware

Current firmware supports:
- RPM adjustment
- duration adjustment
- LCD menu system
- ESC PWM motor control

Additional planned features:
- closed-loop RPM feedback
- coating presets
- automated spin profiles
- data logging
- programmable multi-stage spin cycles

---

# Repository Structure

firmware/      → ESP32 source code
wiring/        → wiring diagrams + pinouts
hardware/      → parts lists + assembly notes
calibration/   → ESC setup + tuning
images/        → build photos
experiments/   → coating and deposition tests
