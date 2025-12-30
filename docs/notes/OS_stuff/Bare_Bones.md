- Cross Compiler is used to know the correct target platform (CPU, operating system)

- Right now for now not developing my own programming language, own compiler, or own bootloader.

# What will we use:
- The GNU Linker from Binutils to link your object files into the final kernel.
- The GNU Assembler from Binutils (or optionally NASM) to assemble instructions into object files containing machine code.
- The GNU Compiler Collection to compile your high level code into assembly.
- The C programming language (or optionally C++) to write the high level parts of your kernel.
- The GRUB bootloader to bootload your kernel using the Multiboot boot protocol that loads us into 32-bit protected mode with paging disabled.
-The ELF as the executable format that gives us control of where and how the kernel is loaded.

# Building a Cross-Compiler
- First thing to do is set up a GCC Cross- Compiler for i686-elf.
- If NOT set up:
    - You will NOT be able to correctly compile your operating system without a cross-compiler.
    - You will NOT be able to correctly compile your operating system without a cross-compiler.
    - You will NOT be able to correctly complete this tutorial with a x86_64-elf cross-compiler, as GRUB is only able to laod 32-bit multiboot kernels. 