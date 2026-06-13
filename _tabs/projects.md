---
title: Projects
icon: fas fa-rocket
order: 4
---

A collection of projects spanning UAV flight controls, systems engineering, bare-metal embedded development, and aerospace simulation.

---

## Self-Balancing Robot — Ada on STM32
*Ongoing · Bare-metal Ada · ARP4754B Methodology*

<img src="https://placehold.co/800x320/1a1a2e/ffffff?text=Ada+%2B+STM32+Blue+Pill+%7C+ARP4754A+%7C+Self-Balancing+Robot"
     alt="Self-Balancing Robot in Ada on STM32"
     style="width:100%; border-radius:8px; margin-bottom:1rem;" />

The most deliberate project in this portfolio. Bare-metal Ada on an **STM32 Blue Pill** using a complete aerospace-grade toolchain: **Alire / gnat_arm_elf 15.2.1 / gprbuild 26.0.1 / libopencm3**.

The engineering discipline is the point — **ARP4754B methodology is applied before implementation**:

1. **FHA (Functional Hazard Assessment)** — Identify failure conditions and assign DALs
2. **PSSA (Preliminary System Safety Assessment)** — Derive architectural safety constraints from FHA
3. **SSA (System Safety Assessment)** — Verification that the implementation satisfies PSSA constraints

This mirrors the process used in real civil aircraft development, applied at embedded system scale. Dual purpose: credible aerospace safety process experience + demonstrable Ada/SPARK Ada capability.

| Aspect | Detail |
|--------|--------|
| **Language** | Ada · SPARK Ada |
| **Hardware** | STM32F103 Blue Pill |
| **Toolchain** | Alire · gnat_arm_elf 15.2.1 · gprbuild 26.0.1 · libopencm3 · OpenOCD |
| **Process** | ARP4754B · FHA · PSSA · SSA · DAL Assignment |
| **Status** | Semihosting output verified · GPIO/LED integration in progress |

---

## PX4 Hybrid VTOL Integration
*Killis Bird LLP · 2024 – 2025*

<img src="https://placehold.co/800x320/0f3460/ffffff?text=PX4+Autopilot+%7C+Hybrid+VTOL+%7C+Flight+Testing"
     alt="PX4 Hybrid VTOL Integration"
     style="width:100%; border-radius:8px; margin-bottom:1rem;" />

End-to-end PX4 autopilot integration for a hybrid VTOL UAV platform. Work spanned software porting to custom Pixhawk-standard hardware, tuning of VTOL transition logic, and structured flight testing.

Key challenges: tuning transition airspeed thresholds, handling thrust vectoring edge cases, and addressing IMU placement to minimise vibration-induced estimation drift.

| Aspect | Detail |
|--------|--------|
| **Stack** | PX4 · NuttX · C++ · Pixhawk · QGroundControl · MAVLink |
| **Platforms** | Hybrid VTOL · Fixed-Wing · Quadcopter |
| **Role** | Full integration, testing, and documentation |

---

## UAV Thrust Stand MBSE
*Killis Bird LLP · 2024 – 2025*

<img src="https://placehold.co/800x320/16213e/ffffff?text=Capella+%2F+ARCADIA+%7C+UAV+Thrust+Stand+MBSE"
     alt="UAV Thrust Stand MBSE in Capella"
     style="width:100%; border-radius:8px; margin-bottom:1rem;" />

Full MBSE treatment of a UAV thrust stand system using **Capella** and the **ARCADIA** methodology, progressing through all four analysis levels:

- **Operational Analysis** — Stakeholder needs, operational activities, actor interactions
- **System Analysis** — System functions, external interfaces, operational to system mapping
- **Logical Architecture** — Functional decomposition, logical components, data flows
- **Physical Architecture** — Physical component allocation, interface definitions

V-model traceability maintained throughout — stakeholder requirements traced to physical test points.

| Aspect | Detail |
|--------|--------|
| **Tools** | Capella · ARCADIA |
| **Deliverables** | OA / SA / LA / PA models · Requirements traceability matrix |
| **Methodology** | V-model · ARCADIA levels |

---

## LQR-Based Quadcopter SIL
*Academic · Madras Institute of Technology*

<img src="https://placehold.co/800x320/1a1a2e/ffffff?text=MATLAB+%2F+Simulink+%7C+LQR+vs+PID+%7C+PX4+SITL"
     alt="LQR vs PID Quadcopter SIL"
     style="width:100%; border-radius:8px; margin-bottom:1rem;" />

Designed and evaluated PID and LQR controllers for a quadcopter in MATLAB/Simulink, then validated both in the PX4 SITL environment. Quantitative comparison across:

- Attitude stabilisation under step disturbances
- Wind gust rejection performance
- Hover and trajectory tracking accuracy
- Control effort and actuator saturation analysis

**Conclusion:** LQR demonstrated superior disturbance rejection with lower steady-state error; trade-off against computational cost documented with metrics.

| Aspect | Detail |
|--------|--------|
| **Stack** | MATLAB · Simulink · PX4 SITL · Gazebo |
| **Controllers** | LQR · PID · State-Space modelling |

---

## BLDC Controller Analysis
*Academic · Madras Institute of Technology*

<img src="https://placehold.co/800x320/0f3460/ffffff?text=MATLAB+%2F+Simulink+%7C+BLDC+%7C+PID+vs+Fuzzy+Logic"
     alt="BLDC Controller Analysis"
     style="width:100%; border-radius:8px; margin-bottom:1rem;" />

Developed and compared PID and Fuzzy Logic Controllers for BLDC motor systems in MATLAB/Simulink. Analysis covered steady-state error, transient response (rise time, settling time, overshoot), and robustness to load variation.

Fuzzy logic showed smoother transient response; PID with proper derivative filtering performed comparably for well-characterised loads — documented with simulation data.

| Aspect | Detail |
|--------|--------|
| **Stack** | MATLAB · Simulink · Fuzzy Logic Toolbox |
| **Controllers** | PID · Fuzzy Logic |

---

## Hybrid Tiltrotor UAV
*Academic / Personal*

<img src="https://placehold.co/800x320/16213e/ffffff?text=Hybrid+Tiltrotor+UAV+%7C+Design+%2B+Fabrication+%2B+Testing"
     alt="Hybrid Tiltrotor UAV"
     style="width:100%; border-radius:8px; margin-bottom:1rem;" />

Designed and fabricated a hybrid UAV using tiltrotor mechanisms, capable of both VTOL and sustained forward-flight. Covered aerodynamic sizing, structural design, tilt servo mechanism design, and flight control mode switching logic.

Documented the VTOL-to-forward-flight transition envelope and identified actuator rate limits as the primary constraint on mode-switching speed.

| Aspect | Detail |
|--------|--------|
| **Disciplines** | UAV Design · Tiltrotor Mechanism · Fabrication · Flight Testing |
| **Validation** | Ground hover stability · Transition envelope mapping |