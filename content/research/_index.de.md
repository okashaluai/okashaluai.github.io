---
title: "Forschung"
eyebrow: "~/research"
description: "Sail2SLEIGH: Überprüfung von Ghidras RISC-V-SLEIGH-Spezifikation anhand des formalen Sail-ISA-Modells."
---
## Sail2SLEIGH

**Masterarbeit, FH Joanneum · in Kooperation mit SBA Research · in Arbeit**

*Überprüfung von Ghidras RISC-V-SLEIGH-Spezifikation anhand des formalen Sail-ISA-Modells.*

Ghidra dekodiert Instruktionen anhand handgeschriebener SLEIGH-Prozessorspezifikationen. Ist eine Spezifikation fehlerhaft, ist jede darauf aufbauende Analyse ebenfalls fehlerhaft – oft unbemerkt. Sail ist ein formales, ausführbares Modell des RISC-V-Befehlssatzes.

Das Projekt besteht aus zwei Teilen:

- **Übersetzung:** ein Tool, das Ghidra-Prozessordefinitionen automatisch aus dem Sail-Modell erzeugt.
- **Differential Testing:** ein Framework, das von Ghidra dekodierte RISC-V-Instruktionen mit Sail vergleicht, um Dekodierfehler zu finden.

Ergebnisse und Writeups erscheinen hier, sobald die Arbeit voranschreitet.
