# Huxley OS

## Build

```bash
# pacman -S qemu	// or emerge --ask app-emulation/qemu 
$ cargo install xargo bootimage
$ bootimage --target x86_64-unknown-huxley	// or bootimage --target x86_64-huxley
$ qemu-system-x86_64 -drive format=raw,file=bootimage.bin 
```