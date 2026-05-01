# Akkoyun Hardware

Open hardware organization for PCB design, embedded systems, modem boards, industrial interfaces, and production-ready electronics projects.

## Focus

This organization is used to keep hardware repositories systematic, reviewable, and maintainable over time.

Typical work in this space includes:

- PCB and schematic design
- Altium-based hardware development
- embedded and IoT hardware platforms
- modem and communication boards
- industrial interface and field electronics
- design-review and manufacturing documentation
- production handoff preparation

## What Lives Here

Repositories in this organization may represent:

- complete board designs
- hardware platform iterations
- communication and modem modules
- power, interface, or controller boards
- reference templates and shared standards
- supporting engineering documentation for validation and production

## Repository Standard

Hardware repositories in this organization are expected to follow the `Hardware_Template` structure.

Core layout:

- `Design Files/` — editable design source files
- `Documents/` — design notes, reviews, visuals, and validation records
- `Production/` — current curated manufacturing handoff package

Recommended output convention:

- `Design Files/Output/YYYY-MM-DD/`

Reference template:

- [`Hardware_Template`](https://github.com/Akkoyun-Hardware/Hardware_Template)

Naming and classification standard:

- [`KOD-STANDARTLARI.md`](./KOD-STANDARTLARI.md)
- Canonical source: <https://www.akkoyun.net/acik-kaynak/kod-standartlari/>

## Working Principles

- Keep source, documentation, and production outputs clearly separated.
- Preserve dated manufacturing and export snapshots when they matter.
- Keep `Production/` clean and manufacturer-facing.
- Avoid tracking generated junk such as preview, cache, and history artifacts.
- Prefer repeatable structure across all board repositories.
- Keep repositories understandable for both engineering review and production handoff.

## Notes

This organization is evolving into the main home for Akkoyun hardware design work.

## Repository Map

```mermaid
graph TD
    ORG[Akkoyun-Hardware]

    ORG --> TEMPLATE[Hardware_Template]
    ORG --> LEGACY[Electronic_Modules (legacy archive source)]
    ORG --> ORGFILES[.github]

    ORG --> B0[B0XX — MCU Segment]
    B0 --> B001[B001]

    ORG --> B1[B1XX — IoT Segment]
    B1 --> B100[B100]
    B1 --> B101[B101]
    B1 --> B102[B102]
    B1 --> B103[B103]
    B1 --> B104[B104]
    B1 --> B106[B106]
    B1 --> B107[B107]
    B1 --> B108[B108]
    B1 --> B151[B151]
    B1 --> B152[B152]
    B1 --> B153[B153]
    B1 --> B154[B154]
    B1 --> B155[B155]
    B1 --> B182[B182]

    ORG --> B2[B2XX — Metering Segment]
    B2 --> B201[B201]
    B2 --> B202[B202]

    ORG --> B3[B3XX — Input / Interface Segment]
    B3 --> B302[B302]
    B3 --> B303[B303]

    ORG --> B4[B4XX — Driver Segment]
    B4 --> B402[B402]
    B4 --> B403[B403]
    B4 --> B404[B404]

    ORG --> B5[B5XX — Sensor Segment]
    B5 --> B501[B501]
    B5 --> B502[B502]
    B5 --> B503[B503]
    B5 --> B504[B504]
    B5 --> B505[B505]
    B5 --> B506[B506]
    B5 --> B510[B510]
    B5 --> B520[B520]

    ORG --> B6[B6XX — Legacy / Misc Segment]
    B6 --> B601[B601]

    ORG --> B8[B8XX — Power Source Segment]
    B8 --> B801[B801]
    B8 --> B802[B802]

    ORG --> B9[B9XX — Mother Board Segment]
    B9 --> B901[B901]
    B9 --> B902[B902]
    B9 --> B903[B903]
    B9 --> B905[B905]
    B9 --> B910[B910]

    ORG --> PSEG[PXXX — Product / System Repositories]
    PSEG --> P101[P101]
    PSEG --> P401[P401]
    PSEG --> P402[P402]
    PSEG --> P403[P403]
    PSEG --> P511[P511]
    PSEG --> P520[P520]
    PSEG --> P902[P902]
```

This map is intended as a quick visual inventory of the organization structure: board families, product/system repositories, and key supporting repositories.

## 📚 Teknik Referanslar

- [PCB Technical References](./REFERENCES/PCB/README.md)

