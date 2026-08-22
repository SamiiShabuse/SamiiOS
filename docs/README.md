# SamiiOS Documentation

This folder collects operating-system development notes, references, and future implementation guides for SamiiOS.

## Reading Path

1. `notes/OS_stuff/introduction.md`
2. `notes/OS_stuff/getting_started.md`
3. `notes/OS_stuff/Bare_Bones.md`
4. `notes/OS_stuff/GCC_Cross_Compiler.md`
5. `notes/OS_stuff/Building_GCC.md`
6. `notes/x86-64/tutorial_1.md`

## Documentation Goals

- Keep setup steps reproducible.
- Separate notes from implemented features.
- Add commands only after they have been tested.
- Track the reason behind toolchain choices such as QEMU, x86_64, and cross-compilation.

## Future Docs

Planned documentation areas:

- Bootloader and kernel entry
- Linker script walkthrough
- VGA text or serial output
- Memory map and paging notes
- Interrupt descriptor table notes
- Debugging with QEMU and GDB