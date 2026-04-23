# CMOS 8-bit Microprocessor Data Path

An 8-bit CMOS microprocessor data path designed at the transistor and layout level using hierarchical VLSI design methodology. The system integrates an Arithmetic Logic Unit (ALU), a barrel shifter, and an 8×8 SRAM register file to support arithmetic, logic, shift, and storage operations. All functional blocks are synchronized using two non-overlapping clock phases and were optimized for functionality, timing, and layout efficiency.

## Overview

This project implements a complete 8-bit CMOS data path composed of three major blocks:

- **Arithmetic Logic Unit (ALU)** for arithmetic and bitwise logic operations
- **Shifter** for shift-based data manipulation
- **8×8 SRAM Register File** for data storage and operand access

The design follows a **hierarchical approach**, allowing lower-level cells to be reused in higher-level modules for better modularity, layout organization, and verification efficiency.

## Architecture

The data path consists of:

- **Register File**
  - 8×8 SRAM-based storage
  - supports data read and write operations
  - provides operands to the ALU and stores processed results

- **ALU**
  - performs arithmetic and logical operations on 8-bit inputs
  - designed to support core processor-style data manipulation functions

- **Shifter**
  - performs controlled shift operations on ALU output
  - enables additional data transformation before write-back

- **Clocking Scheme**
  - uses **two non-overlapping clock phases**
  - ensures proper synchronization between storage and computation stages

## Design Features

- 8-bit CMOS data path implementation
- Hierarchical transistor-level design
- Full-custom layout development
- Timing-aware datapath organization
- Functional integration of ALU, shifter, and SRAM register file
- Two-phase non-overlapping clock synchronization
- Optimized for:
  - functionality
  - timing
  - layout efficiency

## Design Flow

The project was developed through a standard custom IC design flow:

1. **Schematic Design**
   - transistor-level implementation of each functional block

2. **Hierarchical Integration**
   - construction of larger modules from verified lower-level cells

3. **Layout Design**
   - custom physical layout for ALU, shifter, SRAM register file, and top-level datapath

4. **Verification**
   - functional validation
   - layout-level verification
   - extraction-based analysis

5. **Optimization**
   - refinement for timing and layout efficiency

## Main Blocks

### 1. SRAM Register File
The 8×8 SRAM register file stores internal data used by the data path. It supplies operands to the ALU and accepts processed outputs for write-back. The SRAM structure enables compact and efficient on-chip data storage.

### 2. Arithmetic Logic Unit (ALU)
The ALU performs arithmetic and logic functions required by the data path. It serves as the primary computational block in the processor architecture.

### 3. Shifter
The shifter operates on ALU output and provides bit-shift functionality for additional data manipulation.

## Applications

This project demonstrates core concepts in:

- VLSI design
- CMOS digital circuit design
- hierarchical custom layout
- datapath architecture
- SRAM-based storage design
- timing-aware digital system implementation

## Tools
This project was developed using **Cadence Virtuoso VLSI design tools** for schematic design, layout, and verification.

## Project Goals

The main goals of this project were to:

- design a functional 8-bit CMOS datapath
- integrate computation, shifting, and storage blocks
- implement a clean hierarchical layout structure
- ensure reliable timing with two-phase clocking
- optimize the design for performance and physical efficiency

