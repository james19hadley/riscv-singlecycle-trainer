# ⚡ RISC-V Eintakt-Datapath Trainer

> Interactive browser-based trainer for TU Darmstadt Rechnerorganisation Exam Aufgabe 5.

🌐 **Live Demo:** [https://james19hadley.github.io/riscv-singlecycle-trainer/](https://james19hadley.github.io/riscv-singlecycle-trainer/)

---

## 🎯 Overview

A standalone single-cycle RISC-V processor simulator designed for tracing active datapath connections and deducing control signals.

---

## ⚡ Practice Modes

- **Teil a: Datapath** — Trace and highlight active wires on the schematic. Control signals serve as reference.
- **Teil b: Control Signals** — Deduce and select all 10 control signal values in the table dropdowns.
- **Teil a+b: Full Exam Simulation** — Highlight active wires and deduce all 10 control signals simultaneously.

---

## 📋 Instructions & Exam Sources

| Instruction | Type | Exam Source |
| :--- | :--- | :--- |
| `add t0, t1, t2` | R-Type Add | Übung 5.4 |
| `sub s1, s2, s3` | R-Type Subtract | Core Architecture |
| `slt t0, t1, t2` | R-Type Set Less Than | WiSe 22/23 |
| `and t0, t1, t2` | R-Type Bitwise AND | Core Architecture |
| `addi a0, a1, 32` | I-Type Add Immediate | Core Architecture |
| `slli t2, t0, 2` | I-Type Shift Left | Probeklausur |
| `lw a5, 12(s3)` | I-Type Load Word | SoSe 25 |
| `lb t1, 4(s2)` | I-Type Load Byte | Same datapath as lw |
| `sw t0, 8(s1)` | S-Type Store Word | Probeklausur |
| `sb t3, 1(a0)` | S-Type Store Byte | Same datapath as sw |
| `beq Taken` | B-Type Branch Equal | WiSe 25/26 |
| `beq Not Taken` | B-Type Branch Equal | Fallthrough case |
| `bne Taken` | B-Type Branch Not Equal | Übung 5.4 |
| `bne Not Taken` | B-Type Branch Not Equal | Fallthrough case |
| `jal ra, func` | J-Type Jump and Link | SoSe 24 |

---

## 🔍 Features

- **Interactive Tooltip System** — Hover over any hardware unit, wire, or signal value to inspect its function and bit configuration. Global toggle via the header button.
- **Visual Feedback** — Immediate color-coded evaluation using green for correct wires, red for false extras, and orange dashed lines for missed paths.
- **Wire Tracing** — Click to toggle active wire highlight with neutral gray hover overlays.
- **Draggable Split View** — Freely adjust the divider between the schematic and the control table.
- **Single-File Architecture** — Self-contained HTML5 and SVG application with zero external runtime dependencies.

---

## 📚 References

- TU Darmstadt Rechnerorganisation Vorlesung, Teil 2, Folien 26–58
- TU Darmstadt Übungsblatt 5, Aufgabe 5.4
- TU Darmstadt Probeklausur SoSe 2026, Aufgabe 5
- TU Darmstadt Klausur WiSe 2025/2026, Aufgabe 5
- TU Darmstadt Klausur SoSe 2025, Aufgabe 5
- TU Darmstadt Klausur SoSe 2024, Aufgabe 5
- TU Darmstadt Klausur WiSe 2022/2023, Aufgabe 5
- David Money Harris & Sarah L. Harris: *Digital Design and Computer Architecture: RISC-V Edition*, Chapter 7, Section 7.3
