# RISCV_Pipeline_Core
This repository contains the design files of RISC-V Pipeline Core

A 5-stage pipelined **RISC-V (RV32I)** processor implemented in **Verilog HDL**.  
This project simulates instruction-level parallelism and demonstrates how pipelining improves CPU throughput and performance.

---

## 🧠 Overview

This project implements a simplified version of a **RISC-V processor** supporting the **RV32I instruction set** with a **5-stage pipeline architecture**:
1. **Instruction Fetch (IF)**
2. **Instruction Decode (ID)**
3. **Execution (EX)**
4. **Memory Access (MEM)**
5. **Write Back (WB)**

It includes hazard detection, data forwarding, and control logic for efficient pipeline operation.

---

## 🚀 Features

- 🧩 **5-Stage Pipeline** — IF, ID, EX, MEM, WB  
- ⚡ **Hazard Handling** — Implements *data forwarding* and *pipeline stalling*  
- 🧮 **ALU Design** — Supports arithmetic and logical operations  
- 🧠 **Control Unit** — Decodes RISC-V instructions and generates control signals  
- 🔁 **Branch and Jump Handling** — Basic control hazard resolution  
- 💾 **Instruction & Data Memory** — Synchronous memory interface  
- 🧰 **Simulation Support** — Verified using *ModelSim* and *GTKWave*

---

## 🧱 Architecture

```text
        ┌────────┐
        │  IF    │───► Instruction Fetch
        ├────────┤
        │  ID    │───► Instruction Decode
        ├────────┤
        │  EX    │───► Execute (ALU Operations)
        ├────────┤
        │  MEM   │───► Memory Access
        ├────────┤
        │  WB    │───► Write Back
        └────────┘


