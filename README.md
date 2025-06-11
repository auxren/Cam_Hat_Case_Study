# Raspberry Pi Zero 2 W Camera Module Daughterboard

## Overview

This project is a hardware design submission for the Senior Electronics Hardware Engineer case study at Tools for Humanity. It involves the design of a daughterboard for the Raspberry Pi Zero 2 W that integrates:

- IMX219 camera module
- PIR motion sensor
- Ambient light sensor
- Power regulation circuitry
- GPIO and CSI interfacing

The board matches the size and GPIO header configuration of the Raspberry Pi Zero 2 W (65mm x 30mm).

## Features

- IMX219 camera integration via CSI interface  
- Ambient light sensor for lighting-aware imaging  
- PIR motion sensor to trigger camera events  
- Switching regulator-based power supply for high efficiency  
- Direct connection to the Raspberry Pi via GPIO and FFC  
- Test points and layout considerations for testability

## System Requirements

| Component              | Specification                                                  |
|------------------------|----------------------------------------------------------------|
| Camera Module          | IMX219 (IQL-IMX219/FF)                                         |
| PIR Sensor             | Selected for compact form factor and reliable motion detection |
| Ambient Light Sensor   | Tuned for visible spectrum and camera exposure control         |
| Power Input            | 5V 3A DC (via Raspberry Pi USB input)                          |
| Form Factor            | 65mm x 30mm (same as Raspberry Pi Zero 2 W)                    |
| Interfaces             | GPIO header and FFC connector                                  |

## Deliverables

- Schematic Design (KiCad project and PDF)
- PCB Layout (KiCad, Gerber files, and 3D model)
- Bill of Materials (BOM) with part numbers and specifications
- Power Supply Design Document (efficiency and regulator choice justification)
- Design Decision Documentation (component selection and rationale)

## Folder Structure

<pre> <code>
├── EPM
├── Factory
├── Firmware:Software
│   └── TfH_Case_Study_FW_TODO.numbers
├── Hardware
│   ├── Block Diagram
│   ├── Datasheets
│   ├── Power
│   │   └── CamHat_Power_Tracker.numbers
│   ├── TfH_Case_Study
│   │   ├── TfH_Case_Study.kicad_pcb
│   │   ├── TfH_Case_Study.kicad_prl
│   │   ├── TfH_Case_Study.kicad_pro
│   │   ├── TfH_Case_Study.kicad_sch
│   │   └── USB.kicad_sch
│   │   └── .....
│   └── TfH_Case_Study_Pinout_Tracker.numbers
├── Mechanical
│   └── MCOs
├── README.md
└── TfH Case Study - Oren Levy.key
</code> </pre>
