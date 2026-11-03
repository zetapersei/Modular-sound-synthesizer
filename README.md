# Analog Modular Synthesizer

An analog modular synthesizer project inspired by the architecture of classic
synthesizers, including those in the Moog tradition. It grew out of a personal
project I worked on between 1978 and 1980; the schematics preserve that idea
and have since been collected and redrawn in KiCad.

The repository contains the project's electronic design documentation: a
hierarchical top-level schematic, individual module schematics, a PCB project,
and a netlist.

## Modules

| Module | Function |
| --- | --- |
| **VCO** | Voltage-controlled oscillator: generates the basic signal. |
| **VCF** | Voltage-controlled filter, identified in the schematic as the PAiA 4730 filter. |
| **VCA** | Voltage-controlled amplifier: controls the signal level. |
| **ADSR** | Envelope generator for shaping the sound over time. |
| **LFO** | Low-frequency oscillator for slow modulation. |
| **Noise generator** | Noise source for additional timbres and modulation. |
| **Audio mixer** | Combines audio sources. |
| **Keyboard encoder** | Schematic for a 49-key musical keyboard interface. |

The modules are organized in the main schematic
[`analog_synth.kicad_sch`](analog_synth.kicad_sch); each circuit also has its
own separate schematic. Module filenames correspond to the names in the table.

## Opening the project

Open [`analog_synth.kicad_pro`](analog_synth.kicad_pro) in KiCad to access the
project, hierarchical schematic, and PCB
[`analog_synth.kicad_pcb`](analog_synth.kicad_pcb). You can also open the main
schematic file directly.

## Project status

The schematics document the architecture and circuits, but the repository
does not specify whether the hardware has been built or tested. Before building
or powering the circuits, verify the schematics, netlist, footprints,
components, and required voltages.

## License

The project is distributed under the GNU GPL version 3; see [`LICENSE`](LICENSE)
for the full text.
