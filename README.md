# JeongMan v6 Robotic-Arm

A 6-axis robotic arm project developed for the annual academic festival at **Kyungbock High School**. This project covers everything from 3D CAD design and simulation to hardware implementation using an ESP32 and NEMA 23 stepper motors, enhanced by a PyTorch-based neural network for Inverse Kinematics solving.

---

## Project Overview

- **Institution**: Kyungbock High School
- **Event**: 2026 Academic Festival
- **Project Name**: jeongman v6 robot arm
- **Core Focus**: Integrating deep learning-based inverse kinematics with robust hardware using ESP32, NEMA 23 motors, and precise 3D-printed/CAD-designed structures.

---

## System Architecture & Design

### 1. 3D CAD Design (Fusion 360)

The structural components of the robot arm were meticulously designed using **Autodesk Fusion 360**, ensuring optimal weight distribution and structural integrity for the joints.

![CAD Design](assets/cad.png)
_Figure 1: 3D CAD modeling of the jeongman v6 robot arm_

### 2. Workspace & Reachability Analysis

We utilized **Python** to calculate the forward kinematics and visualize the robot's maximum reachable operational space.

![Workspace Analysis](assets/reachable.png)
_Figure 2: Simulated 3D workspace and coordinate reachability_

### 3. Deep Learning-Based Inverse Kinematics (PyTorch)

Instead of traditional geometric calculations, a **PyTorch-based neural network** was trained to predict accurate joint angles ($\theta_0 \sim \theta_4$) for given target coordinates $(X, Y, Z)$. This approach allows for fast, real-time trajectory planning.

![Inverse Kinematics Training](assets/prediction.png)
_Figure 3: Result of inverse kinematics prediction_

---

## Tech Stack & Hardware Specs

### Software & AI

- **CAD & Modeling**: Autodesk Fusion 360
- **AI & Kinematics**: Python, PyTorch

### Hardware & Electronics

- **Main Controller**: ESP32 MCU
- **Actuators**: NEMA 23 Stepper Motors
- **Drivers**: DM556
- **Fabrication**: 3D Printing
