# 🤖 Arduino Line Follower Robot using IR Sensors and L298N Motor Driver

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Arduino-blue">
  <img src="https://img.shields.io/badge/Language-Embedded%20C-orange">
  <img src="https://img.shields.io/badge/Robot-Line%20Follower-success">
  <img src="https://img.shields.io/badge/Motor%20Driver-L298N-red">
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen">
</p>

---

# 📌 Project Overview

This project demonstrates the design and implementation of an **Arduino-based Line Follower Robot** using:
- IR sensors
- L298N motor driver
- DC motors
- Arduino UNO

The robot autonomously follows a black line path by continuously detecting line position using infrared sensors and adjusting motor movement accordingly.

The project focuses on:
- Embedded systems
- Robotics automation
- Sensor interfacing
- Motor control
- Autonomous navigation

---

# 🎯 Objectives

The major objectives of this project are:

- Design an autonomous line follower robot
- Interface IR sensors with Arduino
- Control DC motors using L298N driver
- Implement line tracking logic
- Understand robotic movement control
- Learn real-time sensor processing

---

# 🧠 Introduction

A line follower robot is an autonomous robot that follows a predefined path marked using a black line on a white surface.

The robot uses:
- IR sensors to detect the line
- Arduino UNO for decision making
- L298N motor driver for motor control

Based on sensor outputs, the Arduino controls motor direction and speed to keep the robot aligned with the path.

---

# 🏗️ System Architecture

The robot consists of:

- Arduino UNO
- IR Sensors
- L298N Motor Driver
- DC Motors
- Power Supply
- Switch Module
- Robot Chassis


---

# ⚙️ Hardware Components Used

| Component | Purpose |
|-----------|----------|
| Arduino UNO | Main Controller |
| IR Sensors | Line Detection |
| L298N Motor Driver | Motor Control |
| DC Motors | Robot Movement |
| Wheels | Mobility |
| Battery Supply | Power Source |
| Switch | Power ON/OFF |
| Chassis | Robot Structure |

---

# 🛠️ Software Used

| Software | Purpose |
|----------|----------|
| Arduino IDE | Programming |
| Embedded C/C++ | Code Development |

---

# 📷 Circuit Diagram

The circuit includes:
- Arduino UNO
- Two IR sensors
- L298N motor driver
- Two DC motors
- External power supply

The wiring diagram clearly shows:
- Sensor connections
- Motor driver interface
- Power distribution

---

# 🔥 Fire Detection and Extinguishing System

The robot is integrated with a fire detection and extinguishing mechanism to improve safety and automation capabilities.

The system uses a **Flame Sensor** to continuously monitor fire conditions while the robot performs line following operations. When fire is detected, the robot automatically stops moving and activates a fan-based extinguishing system.

---

# 🧠 Working Principle

The flame sensor continuously checks for the presence of fire.

When a flame is detected:
- The robot immediately stops
- Fan motor turns ON
- Servo motor rotates to scan the fire direction
- Fire extinguishing process begins

This creates an automatic emergency response system.

---

# 📌 Components Used

| Component | Function |
|-----------|-----------|
| Flame Sensor | Detects fire/flame |
| Servo Motor | Rotates to scan flame direction |
| Fan/Coreless Motor | Extinguishes fire |
| Arduino UNO | Controls the system |

---

# 🔥 Flame Detection Logic

The flame sensor output is continuously monitored using Arduino.

```cpp
int flameValue = digitalRead(FLAME_SENSOR);
```

When fire is detected:

```cpp
if(flameValue == LOW)
```

The Arduino identifies the emergency condition and activates the fire response system.

---

# 🛑 Robot Stop Mechanism

Once fire is detected, the robot immediately stops moving.

```cpp
rotateMotor(0,0);
```

This prevents unnecessary movement near the fire source.

---

# 🌬️ Fan Activation

The fan motor automatically turns ON to extinguish the flame.

```cpp
digitalWrite(FAN_PIN,HIGH);
```

The fan blows air toward the fire source to suppress small flames.

---

# 🌀 Servo Motor Scanning

The servo motor rotates to scan different directions for the flame.

```cpp
fireServo.write(40);
fireServo.write(90);
fireServo.write(140);
```

The servo scans:
- Left direction
- Center direction
- Right direction

This helps identify the approximate flame location.

---

# 🚀 Applications

The fire detection system can be used in:

- Industrial Safety Robots
- Fire Rescue Systems
- Smart Automation
- Hazard Monitoring Systems
- Warehouse Safety Monitoring
- Educational Robotics Projects

---

# ✅ Advantages

- Simple implementation
- Low-cost design
- Real-time navigation
- Easy programming
- Compact structure
- Efficient movement control
---

# 👨‍💻 Author

## Adith Soragu
## Allumala Yaswanth
## Likith DK
## K Shobith Kumar

---


