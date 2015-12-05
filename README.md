# kmz80
Z80 Emulator for C written by Mamiya 2006.

See kmz80.txt for detail.

This repository is a fork of kmz80 for some tiny patches below:

- Suppress compiler warnings from modern C compilers.
- Employ [CMake](https://cmake.org) as the build system. 

You can simpley build libkmz80.a with `cmake` as follows.

```
$ git clone https://github.com/okaxaki/kmz80.git
$ cd kmz80
$ make build; cd build
$ cmake ..
$ make
```
