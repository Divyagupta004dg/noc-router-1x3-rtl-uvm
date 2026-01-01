Project Overview



This project implements a 1×3 Network-on-Chip (NoC) Router using SystemVerilog, along with an industry-standard UVM-based verification environment.

The design focuses on scalable RTL architecture, correct packet routing, and robust verification of complex traffic scenarios, similar to interconnect blocks used in modern SoCs.



Why This Project?



Modern SoCs rely heavily on interconnects and NoC routers to move data between IP blocks.

Incorrect routing, poor arbitration, or missing flow control can lead to packet loss, starvation, and hard-to-debug race conditions.



This project addresses those challenges by combining:



Clean RTL design



Proper flow control



Arbitration logic



Coverage-driven UVM verification



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



Tools \& Technologies

Category	Tools / Languages

RTL Design	SystemVerilog

Verification	SystemVerilog + UVM

Assertions	SystemVerilog Assertions (SVA)

Simulation	Questa / VCS / Verilator

Waveform Debug	GTKWave

OS	Ubuntu / Linux

(Optional) Synthesis	Yosys / OpenLane

Design \& Verification Flow



Specification and architecture definition



RTL implementation of router, FIFO, and arbiter



Assertion-based checks for protocol correctness



UVM environment development



Directed and random traffic testing



Functional coverage collection



Debug and corner-case validation



Repository Structure

noc-router-1x3-rtl-uvm/

├── rtl/        # Router, FIFO, Arbiter RTL

├── tb/         # UVM testbench

├── sim/        # Simulation scripts

├── docs/       # Specifications and diagrams

├── wave/       # Waveforms and logs

├── Makefile

└── README.md



Key Learning Outcomes



Designed a scalable packet-based interconnect block



Implemented ready/valid flow control and arbitration



Built a professional UVM verification environment



Debugged contention and race-condition scenarios



Applied assertion-based and coverage-driven verification

