# **Magnetic Levitation Using Arduino**

## **Project Overview**

This project demonstrates magnetic levitation using an Arduino-controlled electromagnetic system. The goal is to levitate a magnet in mid-air using feedback from Hall-effect sensors and a PID (Proportional-Integral-Derivative) control system to maintain stability.

## **Table of Contents**
- [Introduction](#introduction)
- [System Components](#system-components)
- [Theory](#theory)
  - [Magnetic Field of a Solenoid](#magnetic-field-of-a-solenoid)
  - [Levitation Equilibrium](#levitation-equilibrium)
- [Circuit Design](#circuit-design)
  - [Current Amplification](#current-amplification)
  - [Sensor Calibration](#sensor-calibration)
- [Control System](#control-system)
  - [PID Control](#pid-control)
  - [Arduino Code](#arduino-code)
- [Calibration](#calibration)
- [Conclusion](#conclusion)
- [References](#references)

---

## **Introduction**

Magnetic levitation (maglev) systems use electromagnetic forces to lift objects against gravity. In this project, we used an Arduino microcontroller to manage the current in a solenoid, which generates a magnetic field to levitate a magnet. The system relies on real-time feedback from Hall-effect sensors to maintain the magnet’s vertical position.

## **System Components**
- **Arduino Uno**
- **Solenoid Coil**
- **TIP112 Darlington Transistor**
- **Hall-effect Sensors (SS495A)**
- **Neodymium Magnet**
- **Operational Amplifier (LM324)**

## **Theory**

### **Magnetic Field of a Solenoid**
The magnetic field (**B**) generated by a solenoid is described by the equation:

```math
B = μ_0 * (N * I) / L
