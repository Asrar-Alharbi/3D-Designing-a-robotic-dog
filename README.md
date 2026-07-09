# 🐕 Quadruped Robot Dog - Preliminary Mechanical Design

This repository contains the preliminary 3D mechanical design and engineering report for a bio-inspired quadruped robot dog. The goal of this project is to explore the mechanical fundamentals, stability criteria, and actuator constraints required to achieve stable robotic walking.


<img width="502" height="487" alt="لقطة شاشة 2026-07-08 013747" src="https://github.com/user-attachments/assets/4ac748be-7566-4d0b-a453-7d29d2b7aa61" />


## 🚀 Project Overview
The prototype was entirely modeled using **Tinkercad**. To give the design a highly structural, modular, and robotic look, it was converted into **Block Mode (Bricks)**. This layout ensures a rigid chassis while optimizing the geometric boundaries for hardware prototyping.

---

## 📊 Engineering & Design Highlights

### 1. Structure & Degrees of Freedom (DoF)
* **Chassis:** A centralized box-style framework engineered to shield internal components (batteries, microcontrollers).
* **Kinematics:** Features **8 Degrees of Freedom (8 DoF)** total ($2 \text{ DoF}$ per leg: Hip Pitch and Knee Pitch) to balance weight and movement efficiency.

### 2. Actuators & Torque Check
* **Selected Motors:** TowerPro MG996R (Metal Gears, $11\text{ kg}\cdot\text{cm}$ stall torque).
* **Worst-Case Leverage Calculation:** $$\tau = F \times r \times \sin(\theta) = 5.9\text{ N} \times 0.08\text{ m} \approx 0.472\text{ N}\cdot\text{m} \implies 4.8\text{ kg}\cdot\text{cm}$$
* **Safety Factor:** $\approx 2.3$ (Highly stable and prevents servo overheating).

### 3. Locomotion Strategy
The robot utilizes a **Static Crawl Gait (Creep Gait)** implementing a strict $3+1$ moving sequence. This guarantees that a **Support Triangle** is maintained at every fraction of a second, keeping the vertical projection of the Center of Mass (COM) safe without needing dynamic balancing sensors.



## 🛠️ Anticipated Mechanical Mitigations
* **Vibration Control:** Tight tolerances and dual-bearing pivots to eliminate joint backlash.
* **Shock Absorption:** Soft rubber dampeners added to the foot tips to cushion landing impacts.
* **COM Security:** Dedicated central locking bay to prevent LiPo battery shifting.
