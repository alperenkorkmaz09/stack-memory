# Stack Memory (Verilog)

## Project Description

This project implements a stack memory using Verilog. The design supports standard stack operations such as push and pop while maintaining Last-In-First-Out (LIFO) behavior.

## Features

* 8-bit data width
* Stack depth of 8 elements
* Push operation (write data into stack)
* Pop operation (read data from stack)
* Full and Empty status signals

## Files

* `stackmemory.sv` → Main design (stack memory implementation)
* `testbench.sv` → Testbench for simulation and verification

## Design Details

The stack uses an internal memory array and a stack pointer (`sp`) to track the top of the stack.

* Push increases stack pointer
* Pop decreases stack pointer
* Full signal is active when stack is full
* Empty signal is active when stack is empty

## Simulation

The design was simulated using EDA Playground.

Waveform analysis confirms:

* Data is pushed correctly into the stack
* Data is popped in reverse order
* LIFO behavior is verified

## Example Behavior

Values pushed: 10, 20, 30
Values popped: 30, 20, 10

This confirms correct stack operation.

## Tools Used

* Verilog / SystemVerilog
* EDA Playground
* EPWave / GTKWave (waveform viewer)

## Author

Alperen Korkmaz
