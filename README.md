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

👉 Key insight:
The novelty is comparison + quantification, not the circuit itself.

3️⃣ Now map THIS exactly to YOUR NoC Router project
What stays SAME (you already have this)

You do NOT need to throw away your project.

You already have:

RTL architecture

Arbitration

Flow control

UVM verification

Stress scenarios

This is stronger than many papers.

What MUST be ADDED (this is the “paper layer”)

Your project needs ONE RESEARCH AXIS, similar to how that paper used area optimization.

Below are industry-relevant research directions for a NoC router.

4️⃣ Choose ONE research problem (this is critical)
✅ BEST & SIMPLE (recommended)
Arbitration strategy impact on latency and fairness

This maps PERFECTLY to industry.

Research question (paper-style):

How does arbitration strategy affect latency, throughput, and starvation in a 1×3 NoC router under contention?

This is real industry pain.

5️⃣ How your paper structure will look (mapped to comparator paper)
I. Introduction

Just like their paper talked about IC area & cost, you talk about:

NoC routers in modern SoCs

Contention and fairness issues

Need for predictable latency

👉 Industry relevance: CPUs, GPUs, AI accelerators

II. Related Work

Like they reviewed diffusion sharing & legging:

You review:

Fixed-priority arbitration

Round-robin arbitration

Starvation problems

(You don’t need many references—3–5 is enough.)

III. Proposed Architecture

This is where your existing work fits perfectly:

1×3 router

FIFO-based buffering

Ready/valid handshake

Two arbitration modes:

Fixed priority

Round-robin

👉 This is your “methodology” section, like their Section III.

IV. Experimental Methodology (VERY IMPORTANT)

This is where most students fail.

You must specify:

Packet size

Traffic pattern

Simulation cycles

Tools used (SystemVerilog + UVM)

Measurement method

Example:

Simulations were performed over 10,000 cycles using constrained-random traffic in a UVM environment.

V. Results and Discussion

This is the heart of the paper, exactly like their graphs.

You must include tables or graphs, for example:

Arbitration	Avg Latency (cycles)	Max Latency	Starvation
Fixed Priority	28	75	Yes
Round Robin	22	40	No

This is your “67.10% area reduction” equivalent.

VI. Conclusion

Like their summary:

What improved

Why it matters

Future work (scaling to N×M router)

6️⃣ Does industry care about this paper?
YES — if framed correctly

Industry relevance:

Interconnect fabrics

NoC routers

Arbitration fairness

Latency predictability

This is MUCH closer to industry reality than the comparator layout paper.

7️⃣ Do you need RTL → GDS for the paper?

❌ NO

The comparator paper needed layout because area was the metric.

Your metrics are:

Latency

Throughput

Fairness

Verification quality

So simulation-based paper is 100% valid.

8️⃣ Final verdict (very important)
Is your project well enough?

✅ YES — architecture-wise

Does it need modification?

✅ YES — add measurement + comparison

Do you need to redesign everything?

❌ NO

Is it publishable?

✅ YES — as a student / conference paper

9️⃣ Exactly how YOU should proceed (step-by-step)

Keep current RTL + UVM

Add one alternative arbitration scheme

Add latency counters

Run simulations under load

Collect numbers

Write paper sections

That’s it.

If you want next (strongly recommended)

I can:

Propose exact paper title

Write Abstract (ready-to-submit)

Create Result tables

Convert your README → IEEE paper outline

Just say:
👉 “convert my project into paper outline”

Sources
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

👉 Key insight:
The novelty is comparison + quantification, not the circuit itself.

3️⃣ Now map THIS exactly to YOUR NoC Router project
What stays SAME (you already have this)

You do NOT need to throw away your project.

You already have:

RTL architecture

Arbitration

Flow control

UVM verification

Stress scenarios

This is stronger than many papers.

What MUST be ADDED (this is the “paper layer”)

Your project needs ONE RESEARCH AXIS, similar to how that paper used area optimization.

Below are industry-relevant research directions for a NoC router.

4️⃣ Choose ONE research problem (this is critical)
✅ BEST & SIMPLE (recommended)
Arbitration strategy impact on latency and fairness

This maps PERFECTLY to industry.

Research question (paper-style):

How does arbitration strategy affect latency, throughput, and starvation in a 1×3 NoC router under contention?

This is real industry pain.

5️⃣ How your paper structure will look (mapped to comparator paper)
I. Introduction

Just like their paper talked about IC area & cost, you talk about:

NoC routers in modern SoCs

Contention and fairness issues

Need for predictable latency

👉 Industry relevance: CPUs, GPUs, AI accelerators

II. Related Work

Like they reviewed diffusion sharing & legging:

You review:

Fixed-priority arbitration

Round-robin arbitration

Starvation problems

(You don’t need many references—3–5 is enough.)

III. Proposed Architecture

This is where your existing work fits perfectly:

1×3 router

FIFO-based buffering

Ready/valid handshake

Two arbitration modes:

Fixed priority

Round-robin

👉 This is your “methodology” section, like their Section III.

IV. Experimental Methodology (VERY IMPORTANT)

This is where most students fail.

You must specify:

Packet size

Traffic pattern

Simulation cycles

Tools used (SystemVerilog + UVM)

Measurement method

Example:

Simulations were performed over 10,000 cycles using constrained-random traffic in a UVM environment.

V. Results and Discussion

This is the heart of the paper, exactly like their graphs.

You must include tables or graphs, for example:

Arbitration	Avg Latency (cycles)	Max Latency	Starvation
Fixed Priority	28	75	Yes
Round Robin	22	40	No

This is your “67.10% area reduction” equivalent.

VI. Conclusion

Like their summary:

What improved

Why it matters

Future work (scaling to N×M router)

6️⃣ Does industry care about this paper?
YES — if framed correctly

Industry relevance:

Interconnect fabrics

NoC routers

Arbitration fairness

Latency predictability

This is MUCH closer to industry reality than the comparator layout paper.

7️⃣ Do you need RTL → GDS for the paper?

❌ NO

The comparator paper needed layout because area was the metric.

Your metrics are:

Latency

Throughput

Fairness

Verification quality

So simulation-based paper is 100% valid.

8️⃣ Final verdict (very important)
Is your project well enough?

✅ YES — architecture-wise

Does it need modification?

✅ YES — add measurement + comparison

Do you need to redesign everything?

❌ NO

Is it publishable?

✅ YES — as a student / conference paper

9️⃣ Exactly how YOU should proceed (step-by-step)

Keep current RTL + UVM

Add one alternative arbitration scheme

Add latency counters

Run simulations under load

Collect numbers

Write paper sections

That’s it.

If you want next (strongly recommended)

I can:

Propose exact paper title

Write Abstract (ready-to-submit)

Create Result tables

Convert your README → IEEE paper outline

Just say:
👉 “convert my project into paper outline”

Sources
