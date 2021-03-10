# Tiny I/O Nice

This is a fork of `ionice` from [util-linux](https://github.com/karelzak/util-linux), in just 324 lines of C code.

* The localization is removed.
* Support for obsolete systems is removed.
* Other than that it's a fully featured drop-in replacement of `ionice`.
* The resulting executable is 18k when built with GCC 10 on Linux. It can also be built with [cxx](https://github.com/xyproto/cxx).
* The source code in `util-linux` have different licenses in different source files.
* This fork is only GPL2 licensed. `util-linux` uses several open source licenses.

## Build

    gcc -O2 -fPIC -fstack-protector-strong -D_GNU_SOURCE main.c -o tinyionice

## Install

    sudo install -Dm755 tinyionice /usr/bin/tinyionice

## General info

* Version: 1.0.0
* License: GPL2
