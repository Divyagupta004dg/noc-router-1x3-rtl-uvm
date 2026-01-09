# 1×3 NoC Router – RTL Design & UVM Verification

This project implements a **1×3 Network-on-Chip (NoC) Router** using **SystemVerilog**, along with an **industry-standard UVM-based verification environment**.  
The design focuses on **scalable RTL architecture**, **correct packet routing**, and **robust verification of complex traffic scenarios**, similar to interconnect blocks used in modern SoCs.

![Image](https://github.com/user-attachments/assets/e135281e-b623-4cbe-a893-ff6167bfb80b)

## Repository Structure

```text
noc-router-1x3-rtl-uvm/
├── rtl/        # Router, FIFO, Arbiter RTL
├── tb/         # UVM testbench
├── sim/        # Simulation scripts
├── docs/       # Specifications and diagrams
├── wave/       # Waveforms and logs
├── Makefile
└── README.md
```

# 1×3 NoC Router – RTL Design & UVM Verification

## Project Overview

This project implements a **1×3 Network-on-Chip (NoC) Router** using **SystemVerilog**, along with an **industry-standard UVM-based verification environment**.  
The design focuses on **scalable RTL architecture**, **correct packet routing**, and **robust verification of complex traffic scenarios**, similar to interconnect blocks used in modern SoCs.

## Why This Project?

Modern SoCs rely heavily on **interconnects and NoC routers** to move data between IP blocks.  
Incorrect routing, poor arbitration, or missing flow control can lead to **packet loss, starvation, and hard-to-debug race conditions**.

This project addresses those challenges by combining:

- Clean RTL design
- Proper flow control
- Arbitration logic
- Coverage-driven UVM verification

## Project Scope

### RTL Design
- Packet-based **1×3 router**
- Header-based destination routing
- Ready/Valid handshake interface
- Output FIFOs with backpressure handling
- Round-robin arbitration for contention resolution

### Verification
- UVM-based testbench
- Transaction-level packet modeling
- Scoreboard-based checking
- Functional coverage
- SystemVerilog Assertions (SVA)

## Tools & Technologies

| Category | Tools / Languages |
|--------|------------------|
| RTL Design | SystemVerilog |
| Verification | SystemVerilog + UVM |
| Assertions | SystemVerilog Assertions (SVA) |
| Simulation | Questa / VCS / Verilator |
| Waveform Debug | GTKWave |
| OS | Ubuntu / Linux |
| (Optional) Synthesis | Yosys / OpenLane |

## Design & Verification Flow

1. Specification and architecture definition  
2. RTL implementation of router, FIFO, and arbiter  
3. Assertion-based checks for protocol correctness  
4. UVM environment development  
5. Directed and random traffic testing  
6. Functional coverage collection  
7. Debug and corner-case validation  

extraa
Project Scope
RTL Design

Packet-based 1×3 router

Header-based destination routing

Ready/Valid handshake interface

Output FIFOs with backpressure handling

Round-robin arbitration for contention resolution

Verification

UVM-based testbench

Transaction-level packet modeling

Scoreboard-based checking

Functional coverage

SystemVerilog Assertions (SVA)

Project Scope
RTL Design

Packet-based 1×3 router

Header-based destination routing

Ready/Valid handshake interface

Output FIFOs with backpressure handling

Round-robin arbitration for contention resolution

Verification

UVM-based testbench

Transaction-level packet modeling

Scoreboard-based checking

Functional coverage

SystemVerilog Assertions (SVA)

Tools & Technologies
Category	Tools / Languages
RTL Design	SystemVerilog
Verification	SystemVerilog + UVM
Assertions	SystemVerilog Assertions (SVA)
Simulation	Questa / VCS / Verilator
Waveform Debug	GTKWave
OS	Ubuntu / Linux
(Optional) Synthesis	Yosys / OpenLane
Design & Verification Flow

Specification and architecture definition

RTL implementation of router, FIFO, and arbiter

Assertion-based checks for protocol correctness

UVM environment development

Directed and random traffic testing

Functional coverage collection

Debug and corner-case validation

Tools & Technologies
Category	Tools / Languages
RTL Design	SystemVerilog
Verification	SystemVerilog + UVM
Assertions	SystemVerilog Assertions (SVA)
Simulation	Questa / VCS / Verilator
Waveform Debug	GTKWave
OS	Ubuntu / Linux
(Optional) Synthesis	Yosys / OpenLane
Design & Verification Flow

Specification and architecture definition

RTL implementation of router, FIFO, and arbiter

Assertion-based checks for protocol correctness

UVM environment development

Directed and random traffic testing
Tools & Technologies
Category	Tools / Languages
RTL Design	SystemVerilog
Verification	SystemVerilog + UVM
Assertions	SystemVerilog Assertions (SVA)
Simulation	Questa / VCS / Verilator
Waveform Debug	GTKWave
OS	Ubuntu / Linux
(Optional) Synthesis	Yosys / OpenLane
Design & Verification Flow

Specification and architecture definition

RTL implementation of router, FIFO, and arbiter

Assertion-based checks for protocol correctness

UVM environment development

Directed and random traffic testing

Functional coverage collection

Debug and corner-case validation

Functional coverage collection

Debug and corner-case validation

Scoreboard-based checking

Functional coverage

SystemVerilog Assertions (SVA)

Tools & Technologies
Category	Tools / Languages
RTL Design	SystemVerilog
Verification	SystemVerilog + UVM
Assertions	SystemVerilog Assertions (SVA)
Simulation	Questa / VCS / Verilator
Waveform Debug	GTKWave
OS	Ubuntu / Linux
(Optional) Synthesis	Yosys / OpenLane
Design & Verification Flow

Specification and architecture definition

RTL implementation of router, FIFO, and arbiter

Assertion-based checks for protocol correctness

UVM environment development

Directed and random traffic testing

Functional coverage collection
