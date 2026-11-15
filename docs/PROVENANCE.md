# Provenance and portfolio claims

Base hardware: [Faketec](https://github.com/gargomoma/fakeTec_pcb), an open-source Meshtastic hardware board by gargomoma, as confirmed by the project owner. The exact upstream revision and local modifications are not yet recorded.

Source snapshot: local Meshtastic project, originally extracted from:
https://github.com/Paulshapwala/kicad-pcb-1/tree/master/meshtastic

Included: schematic, PCB, project settings, existing board images, and custom footprints extracted from the PCB. Machine-specific KiCad session settings, downloaded firmware binaries, and troubleshooting-only schematic previews are excluded.

The original footprint table used absolute paths to unavailable `faketec.pretty` and `easyeda2kicad.pretty` folders. Included footprint copies were recovered from the board; original library documentation and licenses were not available during preparation. Extraction does not transfer ownership or change existing rights.

Before making original-design claims or selecting a license, document:

- The original circuit and PCB sources, if adapted from another project.
- Which schematic and layout changes were made by the project owner.
- The sources and license terms of third-party footprints and symbols.
- Which assembly, debugging, firmware, and testing tasks were personally performed.

The current project record supports describing prototype assembly and battery-circuit troubleshooting. It does not yet substantiate a fully validated original hardware design, radio performance, battery-life claims, or custom firmware authorship.
