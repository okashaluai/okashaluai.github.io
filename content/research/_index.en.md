---
title: "Research"
eyebrow: "~/research"
description: "Sail2SLEIGH: verifying Ghidra's RISC-V SLEIGH specification against the formal Sail ISA model."
---
## Sail2SLEIGH

**Master’s thesis, FH Joanneum · in collaboration with SBA Research · in progress**

*Verifying Ghidra’s RISC-V SLEIGH specification against the formal Sail ISA model.*

Ghidra relies on hand-written SLEIGH processor specifications to decode instructions. If a specification is wrong, every analysis built on top of it is wrong too, often without anyone noticing. Sail is a formal, executable model of the RISC-V instruction set.

The project has two parts:

- **Translation:** an automated tool that generates Ghidra processor definitions directly from the Sail model.
- **Differential testing:** a framework that compares RISC-V instruction encodings decoded by Ghidra against Sail, to find decoding discrepancies.

Results and writeups will be published here as the work progresses.
