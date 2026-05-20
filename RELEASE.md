# XOLERIC v0.1.0 - AI-Native Microkernel OS

## What's New
- Custom Rust microkernel (no_std, 27KB)
- Bootable ISO with GRUB2 (29MB)
- XAI system with optimized inference (8.9x faster)
- Model retry daemon for automatic downloads

## Files
- `xoleric-kernel.bin` - Flat kernel binary
- `xoleric-kernel` - ELF kernel image  
- `xoleric-microkernel.iso` - Bootable ISO

## Quick Start
```bash
# Boot in QEMU
qemu-system-x86_64 -cdrom xoleric-microkernel.iso -m 512M

# Or run kernel directly
qemu-system-x86_64 -kernel xoleric-kernel -m 512M
```

## XAI Fast Mode
```bash
# Optimized model at 21s response (vs 187s cold start)
xai-fast "your question"
```

## Build from Source
```bash
cd kernel
cargo build --target x86_64-unknown-none -Z build-std=core,alloc --release
bash link-kernel.sh
```
