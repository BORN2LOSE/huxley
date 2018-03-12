# Huxley OS

[![Build Status](https://travis-ci.org/BORN2LOSE/huxley.svg?branch=master)](https://travis-ci.org/BORN2LOSE/huxley) [![dependency status](https://deps.rs/repo/github/BORN2LOSE/huxley/status.svg)](https://deps.rs/repo/github/BORN2LOSE/huxley)

## Build

```bash
# pacman -S qemu	// or emerge --ask app-emulation/qemu 
$ cargo install xargo bootimage
$ bootimage --target x86_64-unknown-huxley	// or bootimage --target x86_64-huxley
$ qemu-system-x86_64 -drive format=raw,file=bootimage.bin 
```