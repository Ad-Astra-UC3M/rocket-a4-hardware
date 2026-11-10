View this project on [CADLAB.io](https://cadlab.io/project/30721). 

# Rocket A4 — Hardware

KiCad hardware for the Ad Astra UC3M Rocket A4 project. One folder per board.

| Folder | Contents |
|---|---|
| `flight-computer/` | KiCad project of the flight computer (`.kicad_pro`, `.kicad_sch`, `.kicad_pcb`, project libraries) |
| `ground-station/` | KiCad project of the ground station |
| `docs/` | Datasheets and design decisions |
| `miscellaneous/` | Test boards and experiments not part of the flight design (e.g. `PCB_A4_v2`, first PCB test) |
## Rules
- Each board folder contains a `production/` subfolder (Gerbers, drill files, BOM) **only** when a revision is sent to fabrication. These files are exported from KiCad, never edited by hand.
- KiCad temporary and per-user files are excluded via `.gitignore`.
- Changes go into `main` through a pull request. Review schematic/PCB diffs on CADLAB.
- Workflow guide: see the Ad Astra version control document.
