# kmz80
Z80 Emulator for C written by Mamiya 2006.

See kmz80.txt for detail.

This repository is a fork of kmz80 for some tiny patches below:

- Eleminate some compiler wraning when with modern C compilers.
- Added CMake build settings. 

You can simpley build libkmz80.a with CMake as follows.

```
$ git clone https://github.com/okaxaki/kmz80.git
$ cd kmz80
$ make build; cd build
$ cmake ..
$ make
```
