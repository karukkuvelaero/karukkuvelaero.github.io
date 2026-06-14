---
title: Projects
icon: fas fa-rocket
order: 4
---

> These projects reflect what I have actually built and where I currently am with each. Progress notes are honest — I would rather show real work in progress than a polished description of something incomplete.
{: .prompt-info }

---

## Self-Balancing Robot — Ada on STM32
*Ongoing · Bare-metal Ada · ARP4754A (learning)*

![Ada STM32](https://placehold.co/800x320/1a1a2e/ffffff?text=Ada+%2B+STM32+Blue+Pill+%7C+Bare-metal+%7C+Learning+ARP4754A)

A personal project with two parallel goals: learning **Ada/SPARK Ada** as a language and learning **ARP4754A** as a process — by applying both to the same system before writing production code.

**Where I actually am:**
- Toolchain fully set up: Alire, gnat_arm_elf 15.2.1, gprbuild 26.0.1, libopencm3, OpenOCD
- Semihosting output verified on Blue Pill hardware
- GPIO/LED verification next step
- ARP4754A process: reading and drafting FHA — not complete, not validated

**What I am learning from this:**
The discipline of asking "what are the failure conditions and their consequences" before deciding on architecture. That is what FHA forces. I am not claiming to have done this professionally — I am doing it deliberately on a personal project so I understand the reasoning, not just the terminology.

| Aspect | Status |
|--------|--------|
| Ada toolchain on STM32 | ✅ Working |
| Semihosting / debug output | ✅ Verified |
| GPIO / peripheral control | 🔄 In progress |
| ARP4754A FHA draft | 🔄 In progress |
| PSSA / SSA | ⏳ Not started yet |

---

## PX4 Hybrid VTOL Integration
*Killis Bird LLP · 2024 – 2025 · Professional work*

![PX4 VTOL](https://placehold.co/800x320/0f3460/ffffff?text=PX4+Autopilot+%7C+Hybrid+VTOL+%7C+Flight+Testing)

End-to-end PX4 integration on a hybrid VTOL platform. This is genuine professional work — not a simulation or academic exercise.

Covered software porting to custom Pixhawk-standard hardware, VTOL transition logic tuning, and structured flight tests across fixed-wing and multirotor modes. Key challenge was tuning transition airspeed thresholds and addressing IMU placement issues causing vibration-induced estimation drift.

| Aspect | Detail |
|--------|--------|
| **Stack** | PX4 · NuttX · C++ · Pixhawk · QGroundControl · MAVLink |
| **Platforms tested** | Hybrid VTOL · Fixed-Wing · Quadcopter |

---

## UAV Thrust Stand MBSE
*Killis Bird LLP · 2024 – 2025 · Professional work*

![MBSE Capella](https://placehold.co/800x320/16213e/ffffff?text=Capella+%2F+ARCADIA+%7C+UAV+Thrust+Stand)

Full MBSE treatment of a UAV thrust stand system using Capella and the ARCADIA methodology — operational, logical, and physical architectures with V-model traceability from stakeholder requirements through to physical test points.

This is the project I can discuss in most depth technically — architecture decisions, traceability rationale, and the gap between what stakeholders said they needed and what the system analysis revealed.

| Aspect | Detail |
|--------|--------|
| **Tool** | Capella · ARCADIA |
| **Levels** | OA → SA → LA → PA |
| **Output** | Architecture models · Traceability matrix |

---

## LQR-Based Quadcopter SIL
*Academic · Madras Institute of Technology*

![LQR SIL](https://placehold.co/800x320/1a1a2e/ffffff?text=MATLAB+%2F+Simulink+%7C+LQR+vs+PID+%7C+PX4+SITL)

Designed and compared PID and LQR controllers for a quadcopter in MATLAB/Simulink, then validated both in PX4 SITL. Quantitative comparison across attitude stabilisation, disturbance rejection, and actuator saturation.

LQR showed better disturbance rejection; PID was simpler to tune. Trade-offs documented with simulation data rather than just stated as conclusions.

| Aspect | Detail |
|--------|--------|
| **Stack** | MATLAB · Simulink · PX4 SITL · Gazebo |
| **Controllers compared** | LQR · PID |

---

## BLDC Controller Analysis
*Academic · Madras Institute of Technology*

![BLDC](https://placehold.co/800x320/0f3460/ffffff?text=MATLAB+%2F+Simulink+%7C+BLDC+%7C+PID+vs+Fuzzy+Logic)

Compared PID and Fuzzy Logic Controllers for BLDC motor systems in MATLAB/Simulink. Metrics: steady-state error, rise time, settling time, overshoot, and load variation robustness.

| Aspect | Detail |
|--------|--------|
| **Stack** | MATLAB · Simulink · Fuzzy Logic Toolbox |
| **Controllers** | PID · Fuzzy Logic |

---

## Hybrid Tiltrotor UAV
*Academic / Personal*

![Tiltrotor](https://placehold.co/800x320/16213e/ffffff?text=Hybrid+Tiltrotor+UAV+%7C+Design+%2B+Fabrication)

Designed and fabricated a hybrid VTOL using tiltrotor mechanisms, validated for both hover and forward-flight operation. Covered aerodynamic sizing, structural design, tilt servo mechanism, and mode-switching logic.

| Aspect | Detail |
|--------|--------|
| **Disciplines** | UAV Design · Fabrication · Flight Testing |
| **Key finding** | Actuator rate limits were the primary constraint on transition speed |