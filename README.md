# SamiiOS

SamiiOS is a low-level systems learning project focused on understanding how operating systems boot, initialize hardware-facing structures, and grow from a small kernel into a usable environment.

> Status: early-stage learning repository. The current repo is primarily organized notes and planning material, with implementation work expected to grow around an x86_64 + QEMU target.

## Goals

- Build practical comfort with OS development fundamentals.
- Target x86_64 so the project can use mature tooling, examples, and debugging workflows.
- Use QEMU for fast local boot testing without physical hardware.
- Document the learning path clearly enough that another student can follow it.

## Planned Technical Direction

| Area | Direction |
| --- | --- |
| Target architecture | x86_64 |
| Emulator | QEMU |
| Toolchain | Cross-compiler based workflow |
| Early focus | Boot process, kernel entry, linker scripts, VGA/serial output |
| Later focus | Memory management, interrupts, scheduling, filesystem experiments, shell |

## Repository Layout

```text
.
|-- README.md
`-- docs/
    |-- README.md
    `-- notes/
        |-- OS_stuff/
        `-- x86-64/
```

## Getting Started

Start with the notes in [`docs/README.md`](docs/README.md). The most useful path is:

1. Read the OS introduction notes.
2. Review the x86_64 and bare-bones boot material.
3. Set up QEMU and a cross-compiler toolchain.
4. Add the first bootable kernel milestone.
5. Keep implementation notes tied to reproducible commands.

## Roadmap

| Phase | Milestone |
| --- | --- |
| 1 | Document target architecture, emulator, and toolchain setup |
| 2 | Build a minimal bootable image in QEMU |
| 3 | Print kernel output through VGA text mode or serial |
| 4 | Add linker script, memory map notes, and basic kernel structure |
| 5 | Explore interrupts, paging, heap allocation, and a tiny shell |

## Project Principles

- Learn the fundamentals directly instead of hiding them behind a large framework.
- Keep notes honest about what is working, planned, or experimental.
- Prefer small reproducible milestones over vague feature claims.
- Treat this as a systems portfolio project: clear docs, clear commands, clear limitations.

## Current Status

The repository is being organized as a professional learning log. Implementation milestones should be added only when they can be built, booted, and explained from the README or docs.