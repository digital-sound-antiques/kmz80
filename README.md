# kmz80
Z80 Emulator for C by Mamiya 2006.

The the original source can be found in the NEZplug source package at http://nezplug.sourceforge.net/

This repository is just a copy of the original kmz80 except tiny patches below:

- Change file encoding SJIS to UTF-8.
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
