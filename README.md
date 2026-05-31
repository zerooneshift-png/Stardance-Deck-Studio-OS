<img width="1470" height="923" alt="Capture d’écran 2026-05-31 à 22 33 45" src="https://github.com/user-attachments/assets/a9652db9-4e40-410d-9d72-a6a9bc9bf008" />
# 🌌 Stardance Deck Studio OS

> A full-stack, multi-language simulation playground for designing custom macro pads and programmable stream decks entirely from code.

---

## 🚀 Project Overview

**Stardance Deck Studio OS** is an all-in-one local engineering workspace that unifies frontend hardware UI layout design, a mock operating system backend runtime, automated circuit board netlist compilation, and programmatic 3D CAD rendering. 

This repository serves as a **zero-cost virtual laboratory**. It allows hackers and hardware engineers to experiment with physical device architectures, keymap matrices, and firmware behavior pipelines safely within a sandbox environment before committing to physical prototyping components.

---

## 🛠️ The Architecture & Stack

This project bridges three distinct technical domains across a unified, local development loop:

### 1. 🎛️ Dynamic UI Canvas (HTML5 / Tailwind CSS / JavaScript)
- **Interactive Matrix Resizer:** Shift your macro pad grid proportions dynamically (from a compact `3x4` panel up to a massive `5x6` command deck).
- **Node Property Inspector:** Select individual keys to alter color tag accents, change labels, and configure key binding strings.
- **KMK Core Simulator:** Compiles live configuration data straight into valid CircuitPython/KMK keyboard array formatting structures (`code.py`).
- **Live Diagnostics Widgets:** Feeds live data visualization curves to track CPU and RAM allocations being pumped by the backend.

### 2. ⚡ Local Control Engine (Node.js / Express)
- **Virtual Flash Pipeline:** Captures the frontend's compiled layout matrix payload via asynchronous AJAX endpoints to mimic real USB flash cycles.
- **Hardware Telemetry Loop:** Broadcasts simulated instrument parameters to mimic active, low-level microprocessing motherboard cycles.

### 3. 🔌 Programmatic Blueprints (Python 3 & OpenSCAD)
- **Circuit Schematic (`generate_pcb.py`):** Automatically maps row and column pin nets, tracks diode orientations, and outputs structured hardware circuit track coordinates.
- **Enclosure CAD (`case_blueprint.scad`):** Uses geometric functional code-to-3D algorithms to slice exact standard 14x14mm mechanical switch cutouts directly out of a renderable chassis plate.

---

## 📦 Workspace File Structure

```text
Stardance_Project/
├── package.json          # Dependency configurations & start script keys
├── server.js            # Node.js backend controller engine
├── index.html           # Core dashboard layout UI 
├── app.js               # Application logic, matrix loops & AJAX pipelines
├── style.css            # Layout optimizations & transition styles
├── generate_pcb.py      # Python matrix trace blueprint generator
└── case_blueprint.scad  # OpenSCAD 3D casing mechanical layout script
