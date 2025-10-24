# Xuantie-gcc-elf-newlib-x86_64
Toolchain of RVME, supporting Xuantie MME v0.3.

## How To Use
1. Including Xuantie MME header and pre-defined API in C/C++.
``` c++
#include <thead_matrix.h>
#include "../common/inst.h"  //you can find in tests/cwq/common/inst.h
```
2. The following shell command can help you to compile the C/C++ code and get the test executable file.
``` shell
bin/riscv64-unknown-elf-gcc -march=rv64gc_zfh_xtheadmatrix -g test.c -o test -O2 -lm -static
```
