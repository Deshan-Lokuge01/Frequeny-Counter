# 📡 Analog Frequency Counter
**Precision frequency measurement using LM311 comparator and 7-segment displays**

<div align="center">
  <img src="https://img.shields.io/badge/Core%20IC-LM311-blue" alt="LM311">
  <img src="https://img.shields.io/badge/Range-4%20Digits-green" alt="4-Digit Display">
  <img src="https://img.shields.io/badge/Resolution-1Hz-yellow" alt="1Hz Resolution">
</div>

---

## 📖 Introduction
Analog frequency counters are essential tools in electronic design for communication systems and signal processing. This project implements a practical frequency counter using:

- **LM311 Voltage Comparator** - Signal conditioning
- **7408 AND Gates** - Pulse gating
- **4026 Decade Counters** - Counting & display driving
- **7-Segment Displays** - Human-readable output

### Key Features
✔ 1Hz-9.999kHz measurement range  
✔ 4-digit resolution  
✔ Breadboard and PCB implementations  
✔ Analog-to-digital conversion  

---

## 🛠️ Core Components

| Component | Purpose | Key Specification |
|-----------|---------|-------------------|
| LM311 Comparator | Converts sine waves to square pulses | Open-collector output |
| 7408 AND Gate | Enables pulse counting during 1Hz window | Quad 2-input |
| 4026 Counter | Decade counter + 7-segment driver | 5V operation |
| 7-Segment Display | Visual frequency output | Common cathode |
| 10kΩ Resistor | Pull-up for LM311 | 1/4W tolerance |

---

## 📐 System Design

### Block Diagram
<div align="center">
  <img src="https://github.com/Deshan-Lokuge01/Frequeny-Counter/raw/main/BLock_Diagram_of_Analog_Frequency_Counter.jpg" width="600" alt="System Block Diagram">
</div>

### Circuit Implementations
<div align="center">
  <h4>4-Digit Prototype</h4>
  <img src="https://github.com/Deshan-Lokuge01/Frequeny-Counter/raw/main/Frequency_Counter_For_4_Digits.jpg" width="450" alt="4-Digit Circuit">
  
  <h4>2-Digit PCB Version</h4>
  <img src="https://github.com/Deshan-Lokuge01/Frequeny-Counter/raw/main/Frequency_Counter_For_2_Digits..jpg" width="450" alt="2-Digit Circuit">
</div>

---

## 🖥️ Hardware Results

### Breadboard Implementation
<div align="center">
  <img src="https://github.com/Deshan-Lokuge01/Frequeny-Counter/raw/main/Output_On_Breadboard.jpg" width="500" alt="Breadboard Prototype">
</div>

### Final PCB
<div align="center">
  <img src="https://github.com/Deshan-Lokuge01/Frequeny-Counter/raw/main/PCB_Implimentation_For_Two_Digits.jpg" width="500" alt="PCB Implementation">
  <p>Compact 2-digit version with improved noise immunity</p>
</div>

---

## 📚 Theory of Operation
1. **Signal Conditioning**  
   - LM311 converts input sine waves to digital pulses
   - 10kΩ pull-up ensures proper logic levels

2. **Pulse Gating**  
   - 7408 AND gate enables counting for precise 1-second intervals

3. **Counting & Display**  
   - 4026 ICs increment count for each pulse
   - Drives 7-segment displays directly

---
