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

## Planned Enhancements / Ongoing Work

- Support for multiple arbitration strategies (fixed priority and round-robin)
- Latency and throughput measurement under different traffic patterns
- Starvation and fairness analysis under high contention scenarios
- Extended UVM sequences for stress and corner-case testing
- Coverage-driven verification closure
- (Optional) Synthesis and basic power/performance analysis

These enhancements are intended to further evaluate the router behavior under realistic NoC traffic conditions and to study the impact of arbitration and flow-control strategies.

hat paper is NOT about “comparator RTL”

It is about:

Paper Element	What they actually did
Problem	IC area & cost reduction
Method	Layout optimization techniques
Baseline	Auto-generated layout
Proposal	Diffusion sharing, legging, guard-ring sharing
Metrics	Area (µm²), % reduction
Results	67.10% area reduction
Industry relevance	Cost saving per wafer


gshekejhr hai ye to galat baat hai ye to hona hi toh hai hi nahi lagaa 
bhdghnigvhkkkjggbmmitfcvjuyttgubgjkihbbnkkikmnnccxxfyunbggjkkmbdeyibbvhshkmljgg

 (Optional) Synthesis and basic power/performance analysis

These enhancements are intended to further evaluate the router behavior under realistic NoC traffic conditions and to study the impact of arbitration and flow-control strategies.

hat paper is NOT about “comparator RTL”

It is about:

Paper Element	What they actually did
Problem	IC area & cost reduction
Method	Layout optimization techniques
Baseline	Auto-generated layout
Proposal	Diffusion sharing, legging, guard-ring sharing
Metrics	Area (µm²), % reduction
Results	67.10% area reduction
Industry relevance	Cost saving per wafer

- (Optional) Synthesis and basic power/performance analysis

These enhancements are intended to further evaluate the router behavior under realistic NoC traffic conditions and to study the impact of arbitration and flow-control strategies.

hat paper is NOT about “comparator RTL”

It is about:

Paper Element	What they actually did
Problem	IC area & cost reduction
Method	Layout optimization techniques
Baseline	Auto-generated layout
Proposal	Diffusion sharing, legging, guard-ring sharing
Metrics	Area (µm²), % reduction
Results	67.10% area reduction
Industry relevance	Cost saving per wafer


gshekejhr hai ye to galat baat hai ye to hona hi toh hai hi nahi lagaa 
bhdghnigvhkkkjggbmmitfcvjuyttgubgjkihbbnkkikmnnccxxfyunbggjkkmbdeyibbvhshkmljgg

 (Optional) Synthesis and basic power/performance analysis

These enhancements are intended to further evaluate the router behavior under realistic NoC traffic conditions and to study the impact of arbitration and flow-control strategies.

hat paper is NOT about “comparator RTL”

It is about:

Paper Element	What they actually did
Problem	IC area & cost reduction
Method	Layout optimization techniques
Baseline	Auto-generated layout
Proposal	Diffusion sharing, legging, guard-ring sharing
Metrics	Area (µm²), % reduction
Results	67.10% area reduction
These enhancements are intended to further evaluate the router behavior under realistic NoC traffic conditions and to study the impact of arbitration and flow-control strategies.

hat paper is NOT about “comparator RTL”

It is about:

Paper Element	What they actually did
Problem	IC area & cost reduction
Method	Layout optimization techniques
Baseline	Auto-generated layout
Proposal	Diffusion sharing, legging, guard-ring sharing
Metrics	Area (µm²), % reduction
Results	67.10% area reduction
Industry relevance	Cost saving per wafer


gshekejhr hai ye to galat baat hai ye to hona hi toh hai hi nahi lagaa 
bhdghnigvhkkkjggbmmitfcvjuyttgubgjkihbbnkkikmnnccxxfyunbggjkkmbdeyibbvhshkmljgg

 (Optional) Synthesis and basic power/performance analysis

These enhancements are intended to further evaluate the router behavior under realistic NoC traffic conditions and to study the impact of arbitration and flow-control strategies.

hat paper is NOT about “comparator RTL”

It is about:

Paper Element	What they actually did
Problem	IC area & cost reduction
Method	Layout optimization techniques
Baseline	Auto-generated layout
Proposal	Diffusion sharing, legging, guard-ring sharing
Metrics	Area (µm²), % reduction
Results	67.10% area reduction


It is about:

Paper Element	What they actually did
Problem	IC area & cost reduction
Method	Layout optimization techniques
Baseline	Auto-generated layout
Proposal	Diffusion sharing, legging, guard-ring sharing
Metrics	Area (µm²), % reduction
Results	67.10% area reduction
Industry relevance	Cost saving per wafer


gshekejhr hai ye to galat baat hai ye to hona hi toh hai hi nahi lagaa 
bhdghnigvhkkkjggbmmitfcvjuyttgubgjkihbbnkkikmnnccxxfyunbggjkkmbdeyibbvhshkmljgg

 (Optional) Synthesis and basic power/performance analysis

These enhancements are intended to further evaluate the router behavior under realistic NoC traffic conditions and to study the impact of arbitration and flow-control strategies.

hat paper is NOT about “comparator RTL”

It is about:

Paper Element	What they actually did
Problem	IC area & cost reduction
Method	Layout optimization techniques
Baseline	Auto-generated layout
Proposal	Diffusion sharing, legging, guard-ring sharing
Metrics	Area (µm²), % reduction
Results	67.10% area reduction
mization techniques
Baseline	Auto-generated layout
Proposal	Diffusion sharing, legging, guard-ring sharing
Metrics	Area (µm²), % reduction
Results	67.10% area reduction


It is about:

Paper Element	What they actually did
Problem	IC area & cost reduction
Method	Layout optimization techniques
Baseline	Auto-generated layout
Proposal	Diffusion sharing, legging, guard-ring sharing
Metrics	Area (µm²), % reduction
Results	67.10% area reduction
Industry relevance	Cost saving per wafer



It is about:

Paper Element	What they actually did
Problem	IC area & cost reduction

Paper Element	What they actually did
Problem	IC area & cost reduction

gshekejhr hai ye to galat baat hai ye to hona hi toh hai hi nahi lagaa 
bhdghnigvhkkkjggbmmitfcvjuyttgubgjkihbbnkkikmnnccxxfyunbggjkkmbdeyibbvhshkmljgg

on techniques
Baseline	Auto-generated layout
Proposal	Diffusion sharing, legging, guard-ring sharing
Metrics	Area (µm²), % reduction
Results	67.10% area reduction
Industry relevance	Cost saving per wafer



It is about:

Paper Element	What they actually did
Problem	IC area & cost reduction

Paper Element	What they actually did
Problem	IC area & cost reduction
