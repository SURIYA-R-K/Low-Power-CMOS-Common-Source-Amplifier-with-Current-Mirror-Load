# Design and Simulation of a Low-Power CMOS Common-Source Amplifier  
### Cadence Virtuoso | GPDK 180 nm

---
This project presents the **design and simulation of a low-power CMOS common-source (CS) amplifier** implemented in **Cadence Virtuoso** using the **GPDK 180 nm** technology.  
The amplifier employs a **PMOS current-mirror active load** and **source degeneration** to achieve stable biasing, improved linearity, and controlled gain suitable for low-power applications.

---

## Tools & Technology
- **EDA Tool**: Cadence Virtuoso  
- **Simulator**: Spectre  
- **Technology Node**: GPDK 180 nm  
- **Supply Voltage**: 1.8 V  

---

## Circuit Description
- **Topology**: NMOS Common-Source Amplifier  
- **Load**: PMOS Current-Mirror Active Load  
- **Bias Current**: 50 µA  
- **Load Capacitance**: 700 aF  
- **Linearity Enhancement**: Source degeneration resistor  

The current-mirror load increases the effective output resistance, while source degeneration improves bias stability and linearity at the cost of reduced gain.

---

## Analyses Performed
- **DC Operating Point Analysis**
  - Verified saturation operation of all MOSFETs  
- **AC Small-Signal Analysis**
  - Extracted midband gain and phase margin  
- **Transient Analysis**
  - Verified output swing and time-domain stability  

---

## Performance Summary
| Parameter | Value |
|---------|------|
| Bias Current | 50 µA |
| Load Capacitance | 700 aF |
| Voltage Gain | ~25 dB |
| Phase Margin | ~68° |
| Supply Voltage | 1.8 V |
| Technology | GPDK 180 nm |

The reported gain corresponds to **small-signal AC analysis** with **source degeneration enabled**.

---

Source degeneration improves linearity and stability while reducing overall gain.

---

