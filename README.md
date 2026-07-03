# PCB Guide

## About
A complete, open-source guide to amateur PCB project: From schematic design to a working device.

## Guide Structure & Workflow
This repository walks you through the entire lifecycle of a hardware project, from a blank canvas in KiCad to a functional, firmware-driven device on your desk. The guide is broken down into six main phases:

### PCB Design
This section covers initial component selection and schematic capture, supported by Electrical Rules Checks (ERC) to catch potential circuit errors early. It then guides you through configuring KiCad's Design Rule Checker (DRC) for our specific manufacturer, leading into the hands-on component placement and trace routing.

**Tools:** KiCad 10, git

### Component Sourcing
This section details the final component selection process, focusing on parts that are popular, highly available, and cost-effective for an amateur project. It guides you through navigating real-world stock realities - which often may require revision of the layout and even the schematic - to avoid rare, outdated, or inconvenient options.

**Tools:** Supplier website (DigiKey for this guide)

### Ordering PCBs & Stencils
This section covers exporting and verifying the necessary fabrication artifacts (Gerber and drill files) from KiCad, before walking you through the manufacturing order form on the JLCPCB platform. It explains the default settings needed for our example board while providing some insights on advanced parameters (like layer count and copper thickness) for more complex projects.

**Tools:** KiCad 10 (Fabrication Outputs & Gerber Viewer), Manufacturer website (JLCPCB for this guide)

### Hardware Assembly
This section covers the step-by-step physical assembly of the board, using hot air for surface-mount (SMD) components and a traditional soldering iron for through-hole parts. It also details fabricating the custom wiring required to reliably connect the assembled board with bench equipment.

**Tools:** Hot air station, Soldering iron station, Hand tools (tweezers, wire strippers, crimpers)

### Software
This section covers writing the minimal firmware and basic scripts required to run a "smoke test" on the new hardware. Rather than building complex applications, the focus here is on developing simple C code using the specific MCU SDK to validate the board's core functionality and safely demonstrate its main features.

**Tools:** VS Code, MCU SDK (C), Python (for utility scripting)

### Testing
This section brings the entire project together, starting with the mechanical setup of mounting the hardware for safe bench operation. Then it guides you through flashing the firmware, executing the core tests, and troubleshooting any issues that arise during the initial bring-up.

**Tools:** Debug probe / Programmer, Bench power supply, Multimeter
