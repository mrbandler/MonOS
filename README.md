# MonOS

A bare-metal Rust kernel whose only purpose is to run a web browser. No shell, no desktop, no window manager — just a single pane of glass between hardware and the web.

The name is a play on *mono* (Greek: alone, single) and *OS* — an operating system that does exactly one thing. It's also a nod to *monos*, because this kernel exists in solitude: one app, one purpose, one pane.

This is a learning project in kernel development, not a production OS.

## Goals

- UEFI boot on x86_64
- Framebuffer rendering with bitmap fonts
- PS/2 keyboard and mouse input
- TCP/IP networking via virtio-net
- A minimal HTML/CSS renderer with HTTP support

## Building

Requires just and QEMU with OVMF firmware installed. The Rust toolchain is configured via `rust-toolchain.toml`.

```sh
just run
```
