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

# 📂 Project Structure

```text
Line_Follower_Robot/
│
├── line_follower.ino        # Arduino Source Code
├── circuit_diagram.png      # Circuit Connections
├── robot_images/            # Project Images
├── documentation/           # Reports and Notes
└── README.md                # Documentation
```

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

# 📌 Circuit Connections

The robot uses:
- Two IR sensors for line detection
- L298N motor driver for controlling motors
- Arduino UNO as the central controller

---

# 🔌 Power Supply

```text
7V – 12V DC
```

Power is supplied to:
- Arduino UNO
- Motor Driver
- DC Motors

---

# 📌 IR Sensor Connections

| IR Sensor | Arduino Pin |
|-----------|-------------|
| IR Right | A0 |
| IR Left | A1 |

The sensors detect:
- Black line
- White surface

---

# 📌 Motor Driver Connections

| Motor Driver Pin | Function |
|------------------|----------|
| IN1 | Right Motor Direction |
| IN2 | Right Motor Direction |
| IN3 | Left Motor Direction |
| IN4 | Left Motor Direction |
| ENA | Right Motor Speed |
| ENB | Left Motor Speed |

---

# 🔄 Working Principle

The line follower robot continuously detects the line using IR sensors.

The Arduino reads sensor outputs and controls the motors accordingly.

---

# 🚗 Forward Movement

When:
```text
Both sensors detect the black line
```

The robot moves forward.

---

# ↩️ Left Turn

When:
```text
Left sensor moves away from line
```

The robot turns left to correct its position.

---

# ↪️ Right Turn

When:
```text
Right sensor moves away from line
```

The robot turns right to correct its direction.

---

# 🛑 Stop Condition

When:
```text
Both sensors fail to detect the line
```

The robot stops moving.

---

# 🧩 Arduino Code Logic

The Arduino program:
- Reads sensor values
- Controls motor directions
- Adjusts motor speed


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

# 🚀 Applications

This project can be used in:

- Industrial Automation
- Warehouse Robots
- Automated Guided Vehicles (AGV)
- Smart Transportation
- Robotics Learning
- Educational Projects

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
## Allumala Yashwanth
## Likith DK
## K Shobith Kumar

---


