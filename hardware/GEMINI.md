# GEMINI.md

## Directory Overview

This directory contains the hardware design files for an unbuffered multiple Eurorack module, created in KiCad. The project is split into two main parts: the `mainboard` containing the electronic components and circuitry, and the `faceplate` for the front panel of the module.

The project is for a simple utility module in the Eurorack synthesizer format. An unbuffered multiple (or "mult") splits an incoming signal into multiple copies without any buffering circuitry. This is suitable for splitting CV signals that are not sensitive to slight voltage drops.

## Key Files

### Mainboard (`mainboard/`)

*   `mainboard.kicad_pro`: The main KiCad project file for the mainboard.
*   `mainboard.kicad_sch`: The schematic file, detailing the circuit design.
*   `mainboard.kicad_pcb`: The PCB layout file, for the physical design of the board.
*   `production/`: This directory contains the manufacturing output files (Gerbers, BOM, position files) needed to produce the PCB.
    *   `bom.csv`: The Bill of Materials, listing all components.
    *   `mainboard.zip`: An archive of the Gerber files, which are used to fabricate the PCB.

### Faceplate (`faceplate/`)

*   `faceplate.kicad_pro`: The KiCad project file for the faceplate.
*   `faceplate.kicad_pcb`: The PCB layout file for the faceplate. Note that for faceplates, the "PCB" is often just a piece of FR4 with drill holes and graphics.
*   `faceplate.kicad_sch`: The schematic for the faceplate (likely simple, containing only mounting holes and jacks).

## Usage

These files are intended to be used with the KiCad EDA suite. You can use KiCad to:

*   View and edit the schematic and PCB layout.
*   Generate new manufacturing files.
*   Modify the design of the module.

To get started, open the `.kicad_pro` file for either the `mainboard` or `faceplate` in KiCad.
