# Noise-Robust Speech Command Recognition Using Digital Signal Processing for Wireless Robot Control

A voice-controlled wireless robotic vehicle that uses **Digital Signal Processing (DSP)** and **speech command recognition** to control robot movement in noisy environments.

## Overview

The system captures human speech, processes the audio signal using DSP techniques to reduce noise, recognizes predefined commands, and wirelessly sends the commands to an **ESP32-based robot**.

The robot uses a **TB6612FNG motor driver** to control four N20 DC motors, with two motors connected in parallel on each channel.

## System Flow

```text
Voice Input
    ↓
Noise Reduction & DSP
    ↓
Speech Command Recognition
    ↓
Wireless Communication
    ↓
ESP32
    ↓
TB6612FNG
    ↓
4 × N20 Motors
```

## Features

* Noise-robust speech command recognition
* Digital signal processing for audio preprocessing
* Wireless robot control
* ESP32-based control system
* TB6612FNG dual-channel motor driver
* Four-wheel differential drive
* Supports commands such as **Forward, Backward, Left, Right, and Stop**

## Hardware

* ESP32 Dev Module
* TB6612FNG Motor Driver
* 4 × N20 DC Motors
* 7.4/7.5 V Battery
* 3.3 V Regulator
* Robot chassis and wheels

## Motor Driver Connections

| TB6612FNG | ESP32 |
| --------- | ----- |
| VCC       | 3.3V  |
| GND       | GND   |
| STBY      | D13   |
| AIN1      | D26   |
| AIN2      | D27   |
| PWMA      | D14   |
| BIN1      | D25   |
| BIN2      | D33   |
| PWMB      | D32   |

**Power:** Motor supply (VM) is connected to the battery, while the ESP32 is powered from a regulated 3.3 V supply.

## Objective

The primary objective is to develop a reliable **voice-controlled robotic system** capable of recognizing speech commands even in the presence of environmental noise by applying digital signal processing techniques.

## Project Structure

```text
Noise-Robust-Speech-Command-Recognition/
│
├── audio_processing/
├── speech_recognition/
├── robot_control/
├── esp32/
├── models/
├── dataset/
└── README.md
```

## Applications

* Voice-controlled robotics
* Assistive robotic systems
* Human-machine interaction
* Wireless automation
* Noise-robust speech interfaces

## NOTE: This project is still under development!!
