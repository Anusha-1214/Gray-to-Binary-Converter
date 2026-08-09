# 4-Bit Gray to Binary Converter using Verilog

## Description

This project implements a 4-bit Gray-to-Binary Code Converter using Verilog HDL.

Gray Code is a binary numeral system in which two consecutive values differ by only one bit. This circuit converts a 4-bit Gray Code input into its corresponding 4-bit Binary value.

## Conversion Formula

For a 4-bit Gray input:

```text
B3 = G3
B2 = G3 XOR G2
B1 = G3 XOR G2 XOR G1
B0 = G3 XOR G2 XOR G1 XOR G0
```

## Example

```text
Gray   = 1011
Binary = 1101
```

## Files

* `gray_to_binary.v` — Verilog design module
* `gray_to_binary_tb.v` — Verilog testbench
* `README.md` — Project documentation
* `.gitignore` — Git ignore file

## Simulation

Compile using Icarus Verilog:

```bash
iverilog -o gray_to_binary_sim gray_to_binary.v gray_to_binary_tb.v
```

Run the simulation:

```bash
vvp gray_to_binary_sim
```

The testbench generates a `gray_to_binary.vcd` waveform file that can be viewed using GTKWave.

## Tools Used

* Verilog HDL
* Visual Studio Code
* Icarus Verilog
* GTKWave

## Features

* 4-bit Gray Code input
* 4-bit Binary output
* Combinational logic
* XOR-based conversion
* All 16 input combinations tested
* VS Code compatible

## Author

Add your name here.

