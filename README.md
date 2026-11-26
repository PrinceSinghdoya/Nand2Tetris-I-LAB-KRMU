# Nand2Tetris Part I – From NAND to Tetris

A hands-on implementation of the projects from **Nand2Tetris: The Elements of Computing Systems (Part I)** by Noam Nisan and Shimon Schocken.

This repository documents my journey of building a computer system from the ground up, starting with basic logic gates and progressing towards a complete Hack computer architecture.

## 📚 About Nand2Tetris

Nand2Tetris is an educational course that teaches how computers work by building their hardware and software components step by step.

**Core Learning Areas:**
- Boolean Logic and Digital Circuits
- Combinational and Sequential Logic
- Arithmetic Logic Unit (ALU)
- Memory Architecture
- Computer Architecture
- CPU Design and Hardware Integration

## 📂 Repository Structure

```text
Nand2Tetris-Part-I/
│
├── Project 1 - Boolean Logic/
│   ├── Not.hdl
│   ├── Not16.hdl
│   ├── And16.hdl
│   ├── Or16.hdl
│   ├── Mux16.hdl
│   ├── Or8Way.hdl
│   ├── Mux4Way16.hdl
│   ├── Mux8Way16.hdl
│   ├── DMux4Way.hdl
│   └── DMux8Way.hdl
│
├── Project 2 - Boolean Arithmetic/
│   ├── Add16.hdl
│   ├── Inc16.hdl
│   └── [Other HDL implementations]
│
├── Project 3 - Sequential Logic/
│   ├── a/
│   └── b/
│
├── Project 5 - Computer Architecture/
│   ├── Memory.hdl
│   ├── Computer.hdl
│   └── [Other HDL implementations]
│
└── Capstone Project/
    └── [Capstone implementation]
```

*The directory structure above is illustrative. Adjust filenames and folders to match the actual repository.*

## 🚀 Projects Overview

### Project 1 – Boolean Logic
Implementation of fundamental logic gates and multiplexers using HDL.

**Concepts Covered:**
- Basic Logic Gates (Not, And, Or)
- 16-bit Logic Gates
- Multiplexers and Demultiplexers
- Multi-way Selection Circuits

### Project 2 – Boolean Arithmetic
Building arithmetic circuits using previously implemented logic components.

**Concepts Covered:**
- Half Adder
- Full Adder
- 16-bit Adder
- Incrementer
- Arithmetic Logic Unit (ALU)

### Project 3 – Sequential Logic
Implementation of sequential circuits to understand how computers store and manage data.

**Concepts Covered:**
- Data Flip-Flop (DFF)
- 1-bit Register
- 16-bit Register
- Program Counter (PC)
- RAM Architecture

### Project 5 – Computer Architecture
Integration of hardware components to build the Hack computer.

**Concepts Covered:**
- Memory System
- RAM and Memory Mapping
- CPU Integration
- ROM32K
- Complete Hack Computer

### Capstone Project
A final implementation bringing together concepts learned throughout Nand2Tetris Part I.

**Focus Areas:**
- Hardware Component Integration
- Computer Architecture
- System-Level Design
- HDL Implementation and Testing

## 🛠️ Technologies & Tools

- **Hardware Description Language:** HDL (Nand2Tetris HDL)
- **Simulator:** Nand2Tetris Hardware Simulator
- **Version Control:** Git & GitHub
- **Learning Resource:** The Elements of Computing Systems – Nisan & Schocken

## 🧪 How to Run

1. Clone this repository:

2. Open the project folder.

3. Download and launch the [Nand2Tetris Software Suite](https://www.nand2tetris.org/software).

4. Open the Hardware Simulator.

5. Load the required `.hdl` file.

6. Load its corresponding `.tst` test file.

7. Run the test and verify the output.

## 🎯 Learning Objectives

Through this repository, I aim to:

- Understand the fundamentals of computer hardware.
- Learn how logic gates combine to form complex circuits.
- Understand arithmetic and sequential logic.
- Explore memory organization and CPU architecture.
- Develop a deeper understanding of how computers work internally.

## 📖 Reference

**Book:** The Elements of Computing Systems: Building a Modern Computer from First Principles

**Authors:** Noam Nisan and Shimon Schocken

**Official Website:** https://www.nand2tetris.org/

---

## 👨‍💻 Author

**Prince**

B.Tech Computer Science & Engineering Student

- GitHub: [Your GitHub Profile](https://github.com/princeSinghdoya)
- LinkedIn: [Your LinkedIn Profile](https://www.linkedin.com/in/princesinghdoya/)

---

⭐ If you find this repository useful, consider giving it a star!

*Building a computer from NAND gates, one project at a time.*