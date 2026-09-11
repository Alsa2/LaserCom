# Laser FPGA Hat

## Project Owner

**Name:** Alessandro Salvetti  
**Platform:** Alchitry Au V2 FPGA

## Project Overview

This project is a custom hat board for the **Alchitry Au V2** that interfaces a laser transmitter and a high-speed optical receive path with the FPGA.

The board is intended to handle laser control, convert small high-speed detector current pulses into usable voltage signals, and provide a clean digital output to the FPGA for further processing.

## What I Hope to Learn

- High-speed analog and mixed-signal PCB design
- Laser diode driving and optical signal detection
- High-speed comparator and amplifier design
- FPGA interfacing and digital signal processing

## Current Design

The design currently includes:

- Alchitry Au V2 hat-board interface
- Laser diode drive circuitry
- High-speed transimpedance / amplifier stage
- Input biasing to keep the analog front end within its valid operating range
- High-speed comparator stage for converting the received pulse into a digital FPGA signal

The analog front end is currently being simulated in LTspice. A bias of approximately **0.4 V** has produced the best pulse response so far with limited ringing. The next step is to integrate and test the comparator stage before moving into the PCB layout.

## Major Components

| Component | Purpose |
|---|---|
| Alchitry Au V2 | FPGA processing and control |
| Laser diode | Optical transmitter |
| High-speed op-amp / TIA | Converts detector current pulses to voltage |
| High-speed comparator | Converts analog pulses to FPGA logic |
| Custom PCB | Au V2 hat and analog interface |

## Current Milestones

| Milestone | Status |
|---|---|
| Initial circuit architecture | Complete |
| Analog front-end simulation | In Progress |
| Comparator integration | Next |
| Hat schematic and pinout | In Progress |
| PCB layout | Not Started |
| Hardware testing | Not Started |

## Project Files

This repository will contain:

- KiCad schematic and PCB files
- LTspice simulations
- FPGA source code
- Datasheets
- Test results and documentation

## Project Image

Replace `hero.png` in the repository root with an image of the completed board or current prototype.
