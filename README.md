# Design and Verification of a Gray Code Encoder Processor using Verilog HDL

## Project Overview
This project focuses on the design and verification of a parameterized Gray Code Encoder using Verilog HDL. It converts a 4-bit binary input into its corresponding Gray code using XOR logic.

The conversion is performed using the expression:

gray = bin ^ (bin >> 1)

## Design Description
The design consists of three sub-blocks:

- Sub-block A: Shifts the binary input right by one position.
- Sub-block B: Uses XOR gates to generate the Gray code.
- Sub-block C: Stores the Gray code output using four D flip-flops controlled by clock, reset and enable signals.

## Tools Used
- Verilog HDL
- AMD (Xilinx) Vivado Design Suite 2026.1
- Vivado Simulator (XSim)
- Target Part: xc7a35tcpg236-1 (Artix-7)

## Verification and Results
The design was verified using a self-checking testbench named tb_gray_encoder.v.

All 16 possible 4-bit binary input combinations were tested and compared with their expected Gray code outputs.

- Total Test Cases: 16
- Passed: 16
- Failed: 0
- Errors: 0

## Conclusion
The Gray Code Encoder was successfully designed and verified using Verilog HDL and Vivado Simulator. All 16 input combinations produced the expected Gray code outputs with zero errors.

## Project Files
- Main Verilog Source Code
- Testbench Source Code
- Block Diagrams
- Simulation Results
- Project Report
