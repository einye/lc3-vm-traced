# LC-3 Virtual Machine (Educational Trace Edition)

A complete **LC-3 virtual machine** written in C, based on the excellent tutorial at [jmeiners.com/lc3-vm](https://www.jmeiners.com/lc3-vm/). This version is **designed for learning**: it narrates every instruction in plain English as it executes, showing the opcode, operands, register values, memory locations, and results.

## Requirements

- **C compiler** (`gcc` or `clang`)
- **POSIX / Unix-like OS** - Linux, macOS, or WSL on Windows (the VM uses `termios`, `select`, and `mmap`)

## Build

```bash
# Clone the repo
git clone https://github.com/einye/lc3-vm-traced.git
cd lc3-vm-educational

# Compile
gcc lc3.c -o lc3

# Or with warnings & optimization
gcc -Wall -Wextra -O2 lc3.c -o lc3

# Usage
./lc3 build/<image-file1.obj>
```
## Acknowledgements

This project is based on the excellent LC-3 tutorial by Justin Meiners:

https://www.jmeiners.com/lc3-vm/

The original tutorial walks through writing this same VM from scratch and is one of the best resources available for understanding how a CPU works. If you found this repo useful, go read the tutorial.

Additional background:

Introduction to Computing Systems: From Bits & Gates to C & Beyond — Patt & Patel (the textbook that defines the LC-3)

The original LC-3 spec from UT Austin