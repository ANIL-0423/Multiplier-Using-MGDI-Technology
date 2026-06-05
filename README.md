# Multiplier-Using-MGDI-Technology
Designed a 4-bit multiplier using Modified GDI technology targeting significant reduction in transistor count and power consumption versus CMOS implementations.

# Design of 4-Bit Multiplier Using Modified Gate Diffusion Input (MGDI) Technology

## Overview

This project presents the transistor-level implementation of a low-power 4-bit multiplier based on Modified Gate Diffusion Input (MGDI) technology. The design is inspired by the IEEE conference paper *"Design of 4-Bit Multiplier Using Modified Gate Diffusion Input Technology for Low Power Applications"*.

The objective of this work is to reduce power consumption, propagation delay, and transistor count compared to conventional CMOS and standard GDI-based multiplier architectures.

## Project Objectives

* Design a low-power 1-bit Full Adder using MGDI logic.
* Develop a 4-bit Full Adder architecture using MGDI cells.
* Construct a 4-bit Multiplier using MGDI-based arithmetic blocks.
* Analyze power consumption, propagation delay, and Power-Delay Product (PDP).
* Compare the proposed MGDI design with Conventional CMOS and GDI implementations.

## Tools Used

* Tanner EDA Tool Suite

  * S-Edit (Schematic Design)
  * T-Spice (Circuit Simulation)
  * W-Edit (Waveform Analysis)

## Design Methodology

### Step 1: MGDI Cell Design

The basic Modified Gate Diffusion Input (MGDI) cell was designed using PMOS and NMOS transistors. MGDI logic significantly reduces transistor count while maintaining logic functionality.

### Step 2: XOR Gate Implementation

A compact 4-Transistor XOR gate was developed and verified through transient simulations.

### Step 3: 1-Bit Full Adder Design

The XOR gates and pass transistor logic were combined to implement a 10-Transistor MGDI Full Adder capable of generating SUM and CARRY outputs.

### Step 4: 4-Bit Full Adder Design

Four MGDI Full Adder blocks were cascaded to create a 4-bit adder structure.

### Step 5: 4-Bit Multiplier Development

The complete multiplier architecture was developed using:

* Partial Product Generation
* MGDI Logic Gates
* MGDI Full Adders

### Step 6: Simulation and Verification

Transient analysis was performed using T-Spice to verify:

* Functional correctness
* Power consumption
* Propagation delay
* Power-Delay Product (PDP)

## Results

| Parameter              | Conventional | GDI     | MGDI     |
| ---------------------- | ------------ | ------- | -------- |
| Transistor Count       | 416          | 56      | 40       |
| Power Consumption (mW) | 32.81        | 2.59117 | 1.108961 |
| Delay (s)              | 0.39         | 0.31    | 0.12     |
| PDP                    | 12.7959      | 0.8032  | 0.133075 |

## Key Achievements

* Reduced transistor count by more than 90% compared to conventional implementation.
* Achieved significant reduction in power consumption.
* Reduced propagation delay.
* Improved Power-Delay Product (PDP).
* Suitable for low-power VLSI and IoT applications.

## Repository Structure

```
├── Schematic/
│   ├── MGDI_Cell
│   ├── XOR_4T
│   ├── Full_Adder_10T
│   └── Multiplier_4Bit
│
├── Simulation/
│   ├── Waveforms
│   ├── Power_Analysis
│   └── Delay_Analysis
│
├── Results/
│   ├── Screenshots
│   ├── Comparison_Tables
│   └── Graphs
│
└── README.md
```

## Applications

* Portable Electronics
* IoT Devices
* Battery-Powered Systems
* Digital Signal Processing
* Low-Power VLSI Systems
* Embedded Computing Platforms

## Author

Anil Kumar K
M.Tech (Embedded Systems)
MLR Institute of Technology and Management
Hyderabad, India

## Acknowledgement

This implementation was developed as an academic VLSI research project using Tanner EDA tools. The design methodology follows the concepts presented in the referenced IEEE conference paper while the complete schematic development, simulation setup, waveform verification, and performance analysis were carried out independently.
