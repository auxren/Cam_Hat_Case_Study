# Raspberry Pi Zero 2 W Camera Module Daughterboard

## Overview

![RENDER](https://github.com/auxren/Cam_Hat_Case_Study/blob/main/Mechanical/Cam_Hat_Case_Study_Ortho_Render.png)

This was from a 72hr design challenge / case study for an interview for a Senior Electrical Engineering Role.

## Requirements

- Camera Module: Integrate the IMX219 camera module (IQL-IMX219/FF).
= Motion Detection: Integrate a suitable PIR motion sensor to detect motion to trigger the
camera.
- Lighting Adjustment: Integrate a suitable ambient light sensor that will be later used to
adjust camera settings based on lighting conditions.
- Power Supply: Design a power supply circuit to ensure stable operation. Choose and
justify the power management components used. Use at least one switching regulator in
your design.
- Form Factor: Ensure the daughter board fits within the dimensions of the Raspberry Pi
Zero 2 W (65mm x 30mm).
- Interconnection: The daughter board will connect to the Raspberry Pi Zero 2 W through
the GPIO header. All components, including the camera module, PIR sensor, and
ambient light sensor, must be placed on the daughter board. Additionally, include an FFC
connector on the edge of the daughter board to allow the user to connect an FFC cable
between the daughter board and the CSI interface of the Raspberry Pi Zero W.
- Power Supply: Assume the Raspberry Pi will be powered with a 5V 3A DC power
supply. Consider power losses and efficiencies.


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

- ✅ Schematic Design (KiCad project and PDF)
- ✅ PCB Layout (KiCad, Gerber files, and 3D model)
- ✅ Bill of Materials (BOM) with part numbers and specifications
- ✅ Power Supply Design Document (efficiency and regulator choice justification)
- ✅ Design Decision Documentation (component selection and rationale)

## Folder Structure

<pre> <code>
├── Cam_Hat_Case_Study_Oren_Levy_Presentation.key -- Case study presentation. Open in Apple Keynote.
├── Cam_Hat_Case_Study_Oren_Levy_Presentation.pdf
├── Firmware:Software
│   └── TfH_Case_Study_FW_TODO.numbers -- Document for tracking items FW should be mindful of. Open in Apple Numbers.
├── Hardware
│   ├── Block Diagram
│   │   └── Cam_Hat_Case_Study_Block_Diagram.png -- High level block diagram
│   ├── BOMs
│   │   └── Cam_Hat_Case_Study_PCB_Assembly_BOM.csv -- Assembly BOM
│   ├── Datasheets -- Datasheet PDFs for referencing
│   ├── Pinout Docs
│   │   └── Cam_Hat_Case_Study_Pinout_Tracker.numbers -- Document for tracking pinouts and net names. Open in Apple Numbers.
│   ├── Power
│   │   └── CamHat_Power_Tracker.numbers -- Power calculator document. Open in Apple Numbers.
│   ├── Schematic
│   │   └── Cam_Hat_Case_Study_Schematic.pdf
│   └── TfH_Case_Study -- KiCad Project
├── LICENSE
├── Mechanical
│   ├── Cam_Hat_Case_Study_Model.STEP -- Model of full "product"
│   ├── Cam_Hat_Case_Study_Ortho_Render.png
│   ├── Cam_Hat_Case_Study_Render_Case_Ortho.png
│   ├── Cam_Hat_Case_Study_Side_Render.png
│   └── Subassemblies  -- Folder with dxf and stp files used for assembly
└── README.md
</code> </pre>


## Block Diagram
![BLOCK DIAGRAM](https://github.com/auxren/Cam_Hat_Case_Study/blob/main/Hardware/Block%20Diagram/Cam_Hat_Case_Study_Block_Diagram.png)
