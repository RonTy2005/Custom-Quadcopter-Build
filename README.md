# 🛸 Custom Quadcopter Build

A **DIY quadcopter project** built using the **Radiolink Crossflight flight controller**, **TS100 GPS**, and **FlySky FS-i6S transmitter**.  
This project demonstrates complete drone assembly — including wiring, calibration, GPS setup, and flight tuning — on an **F450 frame** powered by **2200KV brushless motors** and **30A ESCs**.

---

## 📷 Project Overview

This build focuses on understanding **flight controller integration**, **power distribution**, and **stabilized flight using GPS data**.  
Future upgrades include FPV transmission, telemetry data link, and autonomous waypoint missions.

---

## ⚙️ Components Used

| Component                | Specification / Model            | Function                                   |
|--------------------------|----------------------------------|--------------------------------------------|
| Frame                    | F450                             | Main structure holding all parts           |
| Motors                   | 2200KV Brushless Motors          | Provides lift and thrust                   |
| ESCs                     | 30A Electronic Speed Controllers | Controls motor speed                       |
| Flight Controller        | Radiolink Crossflight            | Stabilizes and controls drone movement     |
| GPS Module               | TS100                            | Provides location and navigation data      |
| Battery                  | 5200mAh 3S/4S LiPo               | Power source for motors and electronics    |
| Transmitter & Receiver   | FlySky FS-i6S                    | Sends control signals to flight controller |
| Propellers               | 10x4.5 (Carbon fiber)            | Converts motor torque into lift            |
| Power Distribution Board | 30A Rated                        | Distributes power from battery to ESCs     |

---

## 🔌 Wiring Diagram (Placeholder)

**Wiring Overview:**
- Each **motor** connects to one **30A ESC**.
- **ESC power lines** connect to the **Power Distribution Board (PDB)**.
- **PDB** connects directly to the **LiPo battery**.
- **Signal wires** from ESCs connect to the **Radiolink Crossflight flight controller**.
- **TS100 GPS** connects to the **UART/GPS port** on the flight controller.
- **Receiver (FS-iA6B or iA10B)** connects to the **SBUS/PPM input** of the flight controller.

---

## ⚙️ Pin Connection Summary

| Component           | Connects To              | Port / Pins             |
|---------------------|--------------------------|-------------------------|
| ESC 1 (Front Left)  | Flight Controller        | M1                      |
| ESC 2 (Front Right) | Flight Controller        | M2                      |
| ESC 3 (Rear Right)  | Flight Controller        | M3                      |
| ESC 4 (Rear Left)   | Flight Controller        | M4                      |  
| GPS (TS100)         | Flight Controller        | UART (TX/RX + 5V + GND) |
| Receiver (FS-iA6S)  | Flight Controller        | SBUS / PPM port         |
| Battery             | Power Distribution Board | XT60 Connector          |

---

## 🧠 Features Implemented
- Stable flight with **Radiolink Crossflight FC**
- **GPS Hold** and **Return-to-Home (RTH)** functionality
- **ESC calibration** and throttle range adjustment
- **PID tuning** for smoother flight control
- Power management with 30A ESCs and balanced LiPo setup

---

## 📡 Future Upgrades

- **FPV System:** Add 5.8GHz camera + video transmitter  
- **Telemetry Module:** For real-time flight data on ground station  
- **Autonomous Navigation:** GPS waypoint missions  
- **2-Axis Camera Gimbal:** For aerial photography stabilization  

---

## 🧰 Software and Tools Used

| Tool                               | Purpose                     |       |
|------------------------------------|-----------------------------|
| Radiolink Crossflight Configurator | FC setup and tuning         |
| FlySky FS-i6S Transmitter Config   | Transmitter calibration     |
| Mission Planner                    | Parameter tuning            |
| LiPo Charger                       | Battery maintenance         |
| Multimeter                         | Power testing & calibration |

---

## 🧮 Basic Flight Test Data

| Parameter           | Value                  |
|---------------------|------------------------|
| Average Flight Time | 10–12 min (no payload) |
| Max Current Draw    | ~25A total hover       |
| Hover Throttle      | ~55%                   |
| GPS Accuracy        | ±1.5 meters            |
| Total Weight        | ~1 kg                  | 

---

## 📚 Learnings & Takeaways

- Understanding how ESCs and flight controllers synchronize PWM signals  
- Hands-on tuning of PID values for stable flight  
- Importance of balanced propellers and frame weight distribution  
- Integrating GPS for autonomous and stable hovering  
- Real-world testing of aerodynamics and power efficiency  

---

## 💡 Future Plans

- Add **optical flow sensor** for better indoor stability  
- Implement **Lidar-based obstacle avoidance**  
- Design custom 3D printed frame parts  
- Build an **autonomous object-following mode** using ESP32-CAM  

---

## 🧑‍💻 Author

**Ankur Ghosh**  
🎓 B.Tech in Computer Science Engineering  
💡 Robotics, IoT & Embedded Systems Enthusiast  
🔗 [LinkedIn]([https://linkedin.com/in/YOURUSERNAME](https://www.linkedin.com/in/ankur-ghosh-b5096622a/))  
📧 agisking.ag.2005@gmail.com

---

