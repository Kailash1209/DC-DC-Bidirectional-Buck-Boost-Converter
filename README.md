# ⚡ Bidirectional Buck-Boost DC-DC Converter

## 📌 Overview

This project focuses on the design, simulation, and hardware implementation of a **non-isolated bidirectional synchronous buck-boost DC-DC converter** capable of operating in both charging and discharging modes.

The converter enables **bidirectional power flow** between two DC sources using a four-switch topology and supports:
- Buck operation
- Boost operation
- Buck-Boost operation

The project was developed to study:
- Power electronics converter design
- PWM switching techniques
- Dead-time generation
- Bidirectional energy transfer
- Converter efficiency and waveform analysis
- Hardware implementation challenges

The complete system was designed and validated using:
- MATLAB/Simulink
- Simscape Electrical
- Hardware prototype testing

---

## 👨‍💻 Author

**Kailash**

Department of Electrical Engineering

---

<p align="center">

![MATLAB](https://img.shields.io/badge/MATLAB-Simulink-orange)
![Power Electronics](https://img.shields.io/badge/Power-Electronics-blue)
![DC-DC Converter](https://img.shields.io/badge/DC--DC-Converter-success)
![Buck Boost](https://img.shields.io/badge/Buck--Boost-Bidirectional-important)
![STM32](https://img.shields.io/badge/Controller-STM32-green)
![Hardware](https://img.shields.io/badge/Hardware-Prototype-yellow)
![PWM](https://img.shields.io/badge/PWM-Control-red)
![Simscape](https://img.shields.io/badge/Simscape-Electrical-blueviolet)

</p>

---

# 📚 Table of Contents

1. Introduction
2. Background Theory
3. Converter Topology
4. Operating Principles
5. Component Selection
6. PWM & Switching Strategy
7. Simulation Results
8. Hardware Implementation
9. Challenges Faced
10. Future Improvements
11. Conclusion

---

# 1️⃣ Introduction

Bidirectional DC-DC converters are widely used in:
- Battery Energy Storage Systems (BESS)
- Electric Vehicles (EVs)
- Renewable Energy Systems
- DC Microgrids
- UPS Systems

Unlike conventional converters, bidirectional converters allow energy transfer in both directions:
- Source → Load/Battery
- Battery → Load

This project implements a **4-switch synchronous buck-boost converter** capable of seamless transition between operating modes while maintaining stable output characteristics.

The converter was developed to understand:
- High-frequency switching
- MOSFET gate driving
- Dead-time implementation
- Inductor current behavior
- Converter efficiency
- Practical hardware issues

---

# 2️⃣ Background Theory

## 2.1 Buck Converter

A buck converter steps down the voltage.

\[
V_{out} = D \times V_{in}
\]

Where:
- \(D\) = Duty Cycle

---

## 2.2 Boost Converter

A boost converter increases the voltage.

\[
V_{out} = \frac{V_{in}}{1-D}
\]

---

## 2.3 Bidirectional Converter

A bidirectional converter allows current flow in both directions.

Applications:
- Battery charging/discharging
- Regenerative braking
- Energy storage systems

---

## 2.4 Synchronous Switching

Instead of diodes, MOSFETs are used for:
- Lower conduction losses
- Higher efficiency
- Faster switching
- Bidirectional current capability

---

# 3️⃣ Converter Topology

## 🔷 Four-Switch Bidirectional Buck-Boost Topology

The converter consists of:
- 4 MOSFET switches
- Inductor
- Input capacitor
- Output capacitor
- PWM gate drive circuitry

### Main Features
✅ Bidirectional power flow  
✅ High efficiency  
✅ Compact topology  
✅ Reduced switching losses  
✅ Multiple operating modes  

---

# 4️⃣ Operating Principles

## 4.1 Buck Mode

When input voltage is greater than output voltage:
- Converter operates in buck mode
- Voltage steps down

### Operation
- Two MOSFETs switch complementarily
- Inductor stores and releases energy

---

## 4.2 Boost Mode

When output voltage must be greater than input voltage:
- Converter operates in boost mode
- Voltage steps up

---

## 4.3 Buck-Boost Mode

When voltage levels overlap:
- Converter enters buck-boost mode
- Smooth transition occurs

---

# 5️⃣ Component Selection

## 🔹 MOSFETs
Used for:
- High-speed switching
- Reduced conduction losses
- Bidirectional operation

---

## 🔹 Inductor

The inductor is the main energy storage element.

### Functions
- Current smoothing
- Energy transfer
- Ripple reduction

---

## 🔹 Capacitors

Capacitors are used for:
- Voltage filtering
- Ripple reduction
- Stable output voltage

---

## 🔹 Gate Driver

Gate driver circuitry provides:
- Proper MOSFET switching
- Isolation
- Dead-time implementation

---

# 6️⃣ PWM & Switching Strategy

## PWM Control

PWM pulses are generated for:
- Duty cycle control
- Voltage regulation
- Mode transition

---

## Dead-Time Generation

Dead-time is introduced between switching transitions to prevent:
- Shoot-through
- MOSFET short circuit

### Benefits
✅ Safe switching  
✅ Reduced switching stress  
✅ Improved reliability  

---

# 7️⃣ Simulation Results

## MATLAB/Simulink Model

The converter was simulated using:
- Simulink
- Simscape Electrical

### Simulated Parameters
- Input voltage
- Output voltage
- Inductor current
- Switching waveforms
- PWM pulses

---

## Observed Results

### ✅ Buck Operation
- Stable output voltage
- Continuous inductor current

### ✅ Boost Operation
- Successful voltage step-up

### ✅ Bidirectional Operation
- Smooth transition between modes

---

# 8️⃣ Hardware Implementation

## Hardware Components
- MOSFET switching stage
- Driver circuit
- Inductor
- Capacitors
- DC supply
- Oscilloscope testing

---

## Hardware Validation

The practical setup demonstrated:
- Proper PWM generation
- Successful switching operation
- Stable converter response
- Bidirectional energy transfer

---

# 9️⃣ Challenges Faced

- Dead-time tuning
- MOSFET switching noise
- Inductor heating
- Hardware synchronization
- Gate driver timing
- Switching losses
- Oscilloscope debugging

---

# 🔟 Future Improvements

## Planned Enhancements
- Closed-loop control
- PID controller implementation
- Digital control using STM32/ESP32
- PCB design
- Efficiency optimization
- IoT monitoring
- Protection circuits

---

# 1️⃣1️⃣ Conclusion

A bidirectional synchronous buck-boost DC-DC converter was successfully designed and analyzed using simulation and hardware implementation techniques.

The project provided practical understanding of:
- Power electronics
- Switching converters
- PWM control
- Hardware implementation
- Converter analysis

The system demonstrated successful:
✅ Buck operation  
✅ Boost operation  
✅ Bidirectional power transfer  
✅ Stable switching behavior  

---

# 🛠️ Software Used

- MATLAB
- Simulink
- Simscape Electrical

---


