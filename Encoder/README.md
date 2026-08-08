# 4-to-2 Encoder using Verilog

## Project Description

A 4-to-2 Encoder is a combinational logic circuit that converts one of four active input lines into a 2-bit binary output. It assumes that only one input is HIGH (1) at a time. Encoders are widely used in digital systems for data compression, keyboard encoding, interrupt handling, and communication systems.

This project implements a 4-to-2 Encoder in Verilog HDL and verifies its functionality using a testbench that applies all valid input combinations.

---

## Truth Table

| D3 | D2 | D1 | D0 | Y1 | Y0 |
|----|----|----|----|----|----|
| 0  | 0  | 0  | 1  | 0  | 0  |
| 0  | 0  | 1  | 0  | 0  | 1  |
| 0  | 1  | 0  | 0  | 1  | 0  |
| 1  | 0  | 0  | 0  | 1  | 1  |

---

## Logic Equations

Y1 = D2 | D3

Y0 = D1 | D3

---

## Files

- `encoder4x2.v` – Verilog design
- `encoder4x2_tb.v` – Testbench
- `output.txt` – Expected simulation output
- `README.md` – Project documentation

---

## Software Used

- Icarus Verilog
- ModelSim
- Xilinx Vivado

---

## How to Run

Compile:

```bash
iverilog encoder4x2.v encoder4x2_tb.v
```

Run:

```bash
vvp a.out
```

---

## Expected Output

```
D3 D2 D1 D0 | Y1 Y0
0  0  0  1 | 0  0
0  0  1  0 | 0  1
0  1  0  0 | 1  0
1  0  0  0 | 1  1
```

---

## Applications

- Keyboard Encoding
- Interrupt Handling
- Data Compression
- Communication Systems
- Digital Signal Processing

---

## Author

Your Name