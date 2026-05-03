# 🚀 UART Transmitter & Receiver (Verilog | FSM | Simulation | Synthesis)

## 📌 Overview

This project implements a complete **UART (Universal Asynchronous Receiver Transmitter)** system using Verilog HDL, including both **transmitter (TX)** and **receiver (RX)** modules.

The design follows a standard digital communication protocol with configurable baud rate and is verified through simulation and synthesis.

---

## ⚙️ Features

* UART TX and RX implementation
* Configurable baud rate generator
* Start bit, data bits, stop bit handling
* FSM-based design
* Verified using testbench simulation
* Synthesized with timing analysis

---

## 🧠 Architecture

### UART Frame Format

```text
| Start Bit | 8-bit Data | Stop Bit |
```

---

### 🔹 UART Transmitter (TX)

* Accepts parallel data input
* Converts data into serial stream
* Sends:

  * Start bit (0)
  * Data bits (LSB first)
  * Stop bit (1)

---

### 🔹 UART Receiver (RX)

* Detects start bit
* Samples incoming serial data
* Reconstructs parallel data
* Generates data valid signal

---

## 🔄 FSM Design

### TX States:

* IDLE
* START
* DATA
* STOP

### RX States:

* IDLE
* START
* DATA
* STOP

---

## 📁 Folder Structure

```bash
RTL/ → UART TX and RX design files  
Tb/  → Testbench for verification  
Sim/ → Simulation outputs / waveform  
Syn/ → Synthesis reports  
```

---

## 🔬 Simulation

The UART system is verified using a testbench that transmits and receives data.

👉 Add waveform here:
<img width="1920" height="931" alt="System overview" src="https://github.com/user-attachments/assets/e38e3e82-a346-400e-a373-5092c0a5b824" />

```text
![Waveform](waveform.png)
```

---

## 🏗️ Synthesis

* Synthesized using standard tools
* Timing constraints applied
* Reports generated for:

  * Area
  * Timing

---

## 🛠️ Tools Used

* Verilog HDL
* ModelSim / Vivado
* Synthesis Tool

---

## 📊 Key Learnings

* FSM-based RTL design
* Serial communication protocol (UART)
* Timing and sampling concepts
* Verification using testbench

---

## 📌 Future Improvements

* Add parity bit support
* Support variable data length
* Integrate with FPGA board

---

## 👤 Author

**Pratyush Machcha**

