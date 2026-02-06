# Common Source Amplifier using Cadence Virtuoso (GPDK 180 nm)

## 📌 Overview
This project presents the design, simulation, and analysis of a **CMOS common-source (CS) amplifier** implemented in **Cadence Virtuoso** using the **GPDK 180 nm** technology node.  
The amplifier employs a **PMOS current mirror as an active load** and includes **source degeneration** to improve bias stability and linearity.

This project focuses on understanding **small-signal gain**, **biasing**, and the practical differences between **AC and transient analysis** in analog CMOS amplifiers.

---

## 🔧 Tools & Technology
- **EDA Tool**: Cadence Virtuoso
- **Simulator**: Spectre
- **PDK**: GPDK 180 nm
- **Supply Voltage**: 1.8 V

> Note: Due to PDK licensing restrictions, Cadence design databases are not included.  
> This repository contains schematics, simulation results, and documentation.

---

## 🧠 Circuit Description
- **Topology**: NMOS Common-Source Amplifier  
- **Load**: PMOS Current Mirror (Active Load)  
- **Biasing**: Current mirror biasing  
- **Stability Enhancement**: Source degeneration resistor  

The current mirror load increases output resistance, thereby improving voltage gain, while source degeneration provides better bias stability and linearity.

---

## 📊 Analyses Performed
- **DC Operating Point Analysis**
  - Verified all MOSFETs operate in saturation
- **AC Small-Signal Analysis**
  - Extracted midband gain and frequency response
- **Transient Analysis**
  - Observed time-domain response and signal swing

---

## 📈 Performance Summary
| Parameter | Value |
|---------|------|
| Voltage Gain | ~100 V/V |
| Gain (dB) | ~40 dB |
| Supply Voltage | 1.8 V |
| Load Type | PMOS Current Mirror |
| Technology | GPDK 180 nm |

> The reported gain is obtained from **small-signal AC analysis**, which represents the true amplifier gain.  
> Transient response is used only to verify signal swing and linear operation.

---

## 📐 Gain Theory
The small-signal voltage gain of the CS amplifier is given by:

\[
A_v \approx g_m \left( r_{o,n} \parallel r_{o,p} \right)
\]

Where:
- \( g_m \) is the NMOS transconductance  
- \( r_{o,n}, r_{o,p} \) are the output resistances of NMOS and PMOS  

The use of a current mirror load significantly increases output resistance, enabling high gain.

---

## 📂 Repository Structure
