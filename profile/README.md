# Akkoyun Hardware

Open hardware organization for PCB design, embedded systems, modem boards, industrial interfaces, and production-ready electronics projects.

## Focus

This organization is used to keep hardware repositories more systematic, easier to review, and easier to maintain over time.

Current work typically includes:

- PCB and schematic design
- Altium-based hardware development
- embedded and IoT hardware platforms
- production handoff preparation
- design-review and manufacturing documentation

## Repository Standard

Hardware repositories in this organization are expected to follow the `Hardware_Template` structure.

Core layout:

- `Design Files/` — editable design source files
- `Documents/` — design notes, reviews, visuals, validation records
- `Production/` — current curated manufacturing handoff package

Recommended output convention:

- `Design Files/Output/YYYY-MM-DD/`

Reference template:

- [`Hardware_Template`](https://github.com/Akkoyun-Hardware/Hardware_Template)

## Current Repositories

- [`B101`](https://github.com/Akkoyun-Hardware/B101)
- [`B202`](https://github.com/Akkoyun-Hardware/B202)
- [`B302`](https://github.com/Akkoyun-Hardware/B302)
- [`B182`](https://github.com/Akkoyun-Hardware/B182)

## Working Principles

- Keep source, documentation, and production outputs clearly separated.
- Preserve dated manufacturing/export snapshots when they matter.
- Keep `Production/` clean and manufacturer-facing.
- Avoid tracking generated junk such as preview/history artifacts.
- Prefer repeatable structure across all board repositories.

## Notes

This organization is evolving into the main home for Akkoyun hardware design work.
