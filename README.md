# open-source-spin-coater

A fully open-source, vacuum-chuck spin coater for thin-film fabrication built as a low-cost alternative to commercial spin coaters.

🚧 **Status:** Early development. Not yet complete or ready for use. See [Build Progress](https://github.com/YOUR_USERNAME/spin-coater#build-progress) below for current status.

## Overview

Commercial spin coaters are a common bottleneck for labs, hobbyists, and independent researchers. This project is an attempt to build a fully open hardware, firmware, and software spin coater capable of precise, repeatable spin speeds, at a fraction of the cost.

The instrument is built around a vacuum-chuck substrate holder driven by a sensorless brushless motor, using ESC telemetry for closed-loop RPM feedback and a PID control loop to hold a precise target speed. A Teensy handles low-level control and speed regulation, with an onboard touchscreen for setting and monitoring spin recipes.

## Planned Capabilities

- Closed-loop RPM control, 1,000–6,000 RPM
- Configurable multi-step spin recipes (ramp rate, hold time, speed per step)
- Onboard touchscreen control and status display
- Vacuum chuck substrate holding (functioning with an external vacume pump)

## Build Progress

- [x] Vacuum chuck mechanical design (preliminary)
- [x] Enclosure mechanical design (preliminary)
- [ ] Circuit design and component selection (in progress)
- [ ] Order mechanical, 3D-printed, and electrical parts
- [ ] Firmware
- [ ] Breadboard prototype
- [ ] Breadboard testing & debugging
- [ ] PCB layout
- [ ] Full assembly & validation

<p float="left">
  <img src="docs/images/spin coater section view.png" width="45%" />
  <img src="docs/images/spin coater preliminary design.png" width="45%" />
</p>

## Repository Structure
```
spin-coater/
├── hardware/
│   ├── schematics/          # KiCad schematic files
│   └── cad/                 # Mechanical CAD files (chuck, enclosure)
├── docs/
│   ├── bom/                 # Bill of materials (in progress)
│   ├── circuit_design_notes.md
│   └── mechanical_design_notes.md
└── README.md
```
## Acknowledgments

This design builds on prior open-source spin coater projects, including:

- [Maasi](https://github.com/klotzsch-lab/Maasi) (Klotzsch Lab, HU Berlin) - sensorless motor + ESC telemetry approach
- [Blueprint IoT](https://www.youtube.com/watch?v=gWZm44vas9E) - inspiration for the vacuum chuck design

## License

- Hardware design files: [CERN-OHL-S v2](https://ohwr.org/cern_ohl_s_v2.txt)
- Software and firmware: MIT

## Author

Samuel O'Blenes

GitHub: [@samueloblenes](https://github.com/samueloblenes)

This is a work in progress, design files, firmware, and documentation will be updated as the project develops. Feedback and suggestions are welcome via GitHub Issues.
