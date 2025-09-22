# 🤖 4-DOF MeArm Robotic Arm

This project showcases a **4-DOF robotic arm** built using the **MeArm kit**.  
It performs **pick-and-place tasks** powered by **SG90 servo motors**, controlled with an **Arduino Uno** and a **PCA9685 PWM driver**.  
Power management is handled by a **DC-DC buck converter** (12V → 5V).  
**MATLAB** was used for kinematic analysis, trajectory visualization, and workspace planning.  

---

## ✨ Features
- 🔧 Pre-assembled **MeArm kit** mechanical structure  
- 🎛 **Arduino Uno + PCA9685** control system  
- ⚡ **DC-DC converter** ensures safe 5V power from 12V source  
- 📐 **MATLAB simulations** for motion, kinematics, and trajectory planning  
- 🤖 Smooth and repeatable **pick-and-place operations**  

---

## 🛠 Hardware Components

| Component              | Description                       |
|-------------------------|-----------------------------------|
| **MeArm Kit (4-DOF)**  | Pre-built acrylic structure       |
| **4× SG90 Servo Motors** | For joint actuation              |
| **Arduino Uno**        | Microcontroller board             |
| **PCA9685 PWM Driver** | 16-channel PWM controller         |
| **DC-DC Buck Converter** | Converts 12V input to 5V servos  |
| **12V Battery/Adapter** | Power source                     |
| **Breadboard & Wires** | For prototyping and connections   |

---

## ⚡ Wiring Overview
- Servo Motors → PCA9685 outputs (channels 0–3)  
- PCA9685 → Arduino Uno via **I2C** (A4 = SDA, A5 = SCL)  
- PCA9685 V+ → Powered by **DC-DC buck converter** output (5V)  
- DC-DC Input → External **12V battery/adapter**  
- Common Ground → Shared between **Arduino, PCA9685, and power supply**  

---

## 📐 MATLAB Analysis
- ✅ Defined **DH parameters** for forward & inverse kinematics  
- ✅ Visualized **joint positions** and simulated **end-effector motion**  
- ✅ Performed **trajectory planning** and workspace exploration  
- ✅ Applied **PD computed torque control** for smooth motion evaluation  

---

## 📸 Project Gallery

### Robot Full View
![MeArm Robot](robot_photo.jpg) <!-- replace with your robot photo file -->

### MATLAB Circuit Simulation
![MATLAB Simulation](matlab_simulation.jpg) <!-- replace with your MATLAB circuit image -->

---

## 🚀 How to Run
1. Assemble the **MeArm kit** and connect servos  
2. Wire PCA9685 and Arduino as described in wiring section  
3. Upload the **Arduino code** to the board  
4. Power the system using a **12V adapter → DC-DC → Servos**  
5. Run **MATLAB scripts** to test kinematics and visualize motion  

