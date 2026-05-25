# 🤖 Line Follower Robot with Fire Detection and Extinguishing System

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Arduino-blue">
  <img src="https://img.shields.io/badge/Language-C%2FC%2B%2B-orange">
  <img src="https://img.shields.io/badge/Project-Robotics-success">
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen">
</p>

---

# 📌 Project Overview

This project implements a **Line Follower Robot with Fire Detection and Extinguishing System** using **Arduino**.

The robot is capable of:
- Following a black line path using IR sensors
- Detecting fire using a flame sensor
- Automatically stopping when fire is detected
- Activating a fan to extinguish fire
- Rotating a servo motor to scan the fire direction

The project combines:
- Robotics
- Embedded Systems
- Sensor Interfacing
- Automation
- Fire Safety Concepts

---

# 🎯 Objectives

The main objectives of this project are:

- Design an autonomous line follower robot
- Detect fire using flame sensors
- Automatically activate fire extinguishing mechanism
- Control DC motors using Arduino
- Interface servo motor and sensors
- Understand robotics automation concepts

---

# 🧠 Introduction

Line follower robots are autonomous robots that follow a predefined path using IR sensors.

In this project, additional fire safety functionality is integrated:
- Flame detection
- Automatic stopping
- Fan-based fire extinguishing system

This makes the robot useful for:
- Industrial safety
- Smart automation
- Robotics learning
- Fire monitoring applications

---

# 🏗️ Project Architecture

The system consists of:

- Arduino Controller
- IR Sensors
- Flame Sensor
- Servo Motor
- DC Motors
- Motor Driver Circuit
- Fan/Coreless Motor
- Robot Chassis

---

# 📂 Project Structure

```text
Line_Follower_Robot/
│
├── line_follower.ino       # Arduino Source Code
├── circuit_diagram.png     # Circuit Diagram
├── robot_images/           # Project Images
├── components_list.txt     # Components Used
└── README.md               # Documentation
```

---

# ⚙️ Hardware Components Used

| Component | Purpose |
|-----------|----------|
| Arduino UNO | Main Controller |
| IR Sensors | Line Detection |
| Flame Sensor | Fire Detection |
| Servo Motor | Fire Scanning |
| DC Motors | Robot Movement |
| Motor Driver | Motor Control |
| Fan/Coreless Motor | Fire Extinguishing |
| Robot Chassis | Mechanical Structure |
| Wheels | Movement |

---

# 🛠️ Software Used

| Software | Purpose |
|----------|----------|
| Arduino IDE | Programming |
| Embedded C/C++ | Code Development |

---

# 📌 Pin Configuration

| Component | Pin |
|-----------|-----|
| Right IR Sensor | A0 |
| Middle IR Sensor | A1 |
| Left IR Sensor | A2 |
| Flame Sensor | D2 |
| Servo Motor | D3 |
| Fan Motor | D2 |
| Right Motor Enable | D6 |
| Left Motor Enable | D5 |

---

# 🔄 Working Principle

The robot continuously follows a line using IR sensors while monitoring for fire using a flame sensor.

---

# 🚗 Line Following Operation

The IR sensors detect the black line path.

---

## Forward Movement

```text
Left Sensor = LOW
Right Sensor = LOW
```

Both motors move forward.

---

## Right Turn

```text
Right Sensor = HIGH
Left Sensor = LOW
```

Robot turns right.

---

## Left Turn

```text
Right Sensor = LOW
Left Sensor = HIGH
```

Robot turns left.

---

## Stop Condition

```text
Both Sensors HIGH
```

Robot stops moving.

---

# 🔥 Fire Detection System

The flame sensor continuously monitors fire conditions.

When fire is detected:
- Robot stops immediately
- Fan motor turns ON
- Servo motor scans the fire area
- Fire extinguishing process begins

---

# 🌀 Servo Motor Operation

The servo motor rotates between:
- 40°
- 90°
- 140°

This helps scan the direction of the flame.

---

# 🌬️ Fire Extinguishing Mechanism

A fan/coreless motor is activated when fire is detected.

The fan:
- Blows air toward the flame
- Helps extinguish small fires

---

# 🧩 Code Explanation

---

# 📌 IR Sensor Logic

```cpp
if (rightIRSensorValue == LOW && leftIRSensorValue == LOW)
{
    rotateMotor(MOTOR_SPEED, MOTOR_SPEED);
}
```

Robot moves forward when both sensors detect the line.

---

# 📌 Fire Detection Logic

```cpp
if(flameValue == LOW)
```

LOW signal indicates fire detection.

---

# 📌 Fan Activation

```cpp
digitalWrite(FAN_PIN,HIGH);
```

Turns ON fan motor during fire detection.

---

# 📌 Servo Scanning

```cpp
fireServo.write(40);
fireServo.write(90);
fireServo.write(140);
```

Servo scans different directions to locate fire.

---

# 📌 Motor Control Function

```cpp
rotateMotor(int rightMotorSpeed, int leftMotorSpeed)
```

Controls:
- Robot direction
- Speed
- Turning operations

---

# ▶️ How to Run the Project

## Step 1: Connect Hardware

Connect:
- IR sensors
- Flame sensor
- Motors
- Servo motor
- Fan motor
- Arduino board

---

## Step 2: Upload Code

Open Arduino IDE and upload:

```text
line_follower.ino
```

---

## Step 3: Power the Robot

Provide external power supply to motors and Arduino.

---

## Step 4: Test the Robot

- Place robot on black line track
- Introduce flame source
- Observe automatic fire detection and extinguishing

---

# 📊 Features of the System

- Autonomous line following
- Fire detection capability
- Automatic fire extinguishing
- Servo-based flame scanning
- Real-time sensor processing
- Embedded robotic automation

---

# 🚀 Applications

This project can be used in:

- Industrial Automation
- Fire Safety Systems
- Smart Robotics
- Warehouse Monitoring
- Educational Robotics
- Autonomous Navigation Systems

---

# ✅ Advantages

- Autonomous operation
- Fast fire detection
- Compact robotic design
- Low-cost implementation
- Real-time monitoring
- Easy sensor integration

---

# 📚 Learning Outcomes

Through this project, the following concepts were learned:

- Arduino Programming
- Sensor Interfacing
- Robotics Control
- Embedded Systems
- Motor Driver Control
- Servo Motor Operation
- Fire Detection Systems
- Autonomous Navigation

---

# 🔮 Future Enhancements

The project can be improved further by adding:

- IoT Monitoring
- Bluetooth/WiFi Control
- Camera Integration
- AI-based Navigation
- Smoke Sensors
- Obstacle Avoidance
- Mobile App Control

---

# 👨‍💻 Author

## Adith Soragu

Electronics and Communication Engineering

---

# ⭐ GitHub Repository

If you found this project useful, consider giving it a ⭐ on GitHub.

---

# 📄 License

This project is developed for educational and learning purposes only.
