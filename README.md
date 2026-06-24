# RE-CYD

Open hardware files for RE-CYD, a reworked Cheap Yellow Display (CYD-2432S028) built to run the full [Bruce Firmware](https://github.com/BruceDevices/firmware) module set at once: PN532, NRF24+PA/LNA, CC1101, RDM6300, and IR, on a dedicated power section instead of the CYD's stock regulator.

This repo holds the hardware: PCB design files, 3D-printable case files, bill of materials, and other build resources. Firmware (the board config and Bruce fork) lives in a separate repo, linked below.

Full build writeups, with the actual debugging history, are on [crashlogs.com](https://crashlogs.com).

## Contents

```
RE-CYD/
├── v1/                  Cable-based prototype, breadboard-era build
├── v2/                  PCB-based revision, current stable build
│   ├── pcb/             Gerbers, schematic, BOM
│   └── case/            3D-printable case STLs
├── v3/                  In progress
└── docs/                Photos, reference notes, pinout diagrams
```

Each version folder has its own README with build-specific notes. Start with v2 if you're building one of these yourself, it's the current stable revision.

## Related writeups

- [INCIDENT REPORT: Five Radios, One Cheap Display, Zero Free Pins](https://crashlogs.com/posts/recyd/v1/), V1 build and the GPIO/power/SD-card debugging story
- [INCIDENT REPORT: RE-CYD V2, Trading Cable Spaghetti for a Real PCB](https://crashlogs.com/posts/recyd/v2/), the PCB revision covered in this repo

## Related repos

- [crashlogs/Bruce-Re-CYD](https://github.com/crashlogs/Bruce-Re-CYD), the firmware side: Bruce Firmware fork with the RE-CYD board config

## Status

V2 is the current stable build and what's documented here in most detail. V3 is in progress, see the open issues for what's planned (case clearance, RDM6300 antenna placement, FM5324 status LED routing).

If you build one of these, or get a different CYD firmware running on this hardware (see the V2 writeup for why that might work), open an issue or a discussion, I'd like to hear about it.

## License

Hardware design files (PCB, schematics, case STLs) in this repo are licensed under the [CERN Open Hardware Licence Version 2 - Strongly Reciprocal (CERN-OHL-S-2.0)](LICENSE). See the License section below for what that means in practice.

## Contributing

Issues and pull requests are welcome, especially build reports, fixes, or compatibility notes with other CYD firmware projects.
