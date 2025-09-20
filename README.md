# Autonomous Vehicle Security Simulators

This repository collects references and resources for **simulators used in security research** on autonomous vehicles (AVs).  
We focus on platforms that support **attack modeling** in both **virtual** and **physical** environments.

---

## 🔒 1. MetAdv: Unified Virtual + Physical Adversarial Testing

- **Description**: MetAdv is an interactive adversarial testing platform that unifies **virtual simulations** and **physical vehicle experiments**.  
  It allows dynamic generation of adversarial scenarios and end-to-end evaluation of AV robustness.  
- **Use Cases**:  
  - Perception attacks (camera, LiDAR, multi-sensor spoofing)  
  - End-to-end pipeline robustness testing  
  - Transitioning from simulated attacks to physical testing  
- **Paper**: [MetAdv: A Unified and Interactive Adversarial Testing Platform](https://arxiv.org/abs/2508.06534)  
- **Status**: Research platform (not yet open-sourced).  

---

## 🚙 2. Sim-on-Wheels: Vehicle-in-the-Loop Attack Simulation

- **Description**: Sim-on-Wheels is a **vehicle-in-the-loop framework** that blends a **real vehicle** with **virtual adversarial scenarios**.  
  Virtual objects/events can be injected into real sensor streams to safely evaluate AV resilience.  
- **Use Cases**:  
  - Adversarial object insertion (fake pedestrians, cars)  
  - Safety-critical corner case testing without real-world danger  
  - Combining real dynamics with simulated attack conditions  
- **Paper**: [Sim-on-Wheels: A Vehicle-in-the-Loop Framework for Testing Autonomous Systems](https://arxiv.org/abs/2306.08807)  
- **Status**: Research framework, prototypes demonstrated in academia.  

---

## 🏙️ 3. CARLA: Baseline Simulator for Security & Resilience Research

- **Description**: CARLA is the most widely used **open-source simulator** for autonomous driving research.  
  While not designed specifically for attacks, it is commonly used to study adversarial scenarios.  
- **Use Cases**:  
  - Adversarial patches on traffic signs  
  - Sensor spoofing (camera, LiDAR)  
  - Testing detection, planning, and control resilience under attack  
  - Large-scale scenario simulation for security and safety  
- **Links**:  
  - Website: [https://carla.org](https://carla.org)  
  - GitHub: [https://github.com/carla-simulator/carla](https://github.com/carla-simulator/carla)  
- **Status**: Open-source, ROS/Autoware compatible, large community support.  
https://www.youtube.com/watch?v=AZMdYPN6_Mc
---

## 📊 Summary

| Simulator        | Virtual Support | Physical Integration | Typical Use in Security Research |
|------------------|-----------------|----------------------|----------------------------------|
| **MetAdv**       | ✅ Yes          | ✅ Yes               | Adversarial testing across domains |
| **Sim-on-Wheels**| ⚠️ Partial      | ✅ Yes               | Vehicle-in-loop, mixed reality attacks |
| **CARLA**        | ✅ Yes          | ⚠️ Indirect (via ROS/transfer) | Perception & planning attack testing |

---

## 📂 How to Use This Repo

This repository is a **reference collection**.  
- For CARLA: clone and run the simulator ([docs](https://carla.readthedocs.io)).  
- For MetAdv & Sim-on-Wheels: see linked research papers for setup and experiment design.  

We encourage contributions: if you know of other **attack-oriented simulators** or have code for reproducing these works, feel free to open an issue or PR.

---
