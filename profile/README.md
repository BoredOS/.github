<div align="center">
  <img src="https://raw.githubusercontent.com/BoredOS/BoredOS/refs/heads/main/branding/bOS_full_gradient_cropped.png" alt="BoredOS Logo" width="450" />

  <h3>A modern x86_64 hobbyist operating system built from the ground up.</h3>

  [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
  ![Platform: x86_64](https://img.shields.io/badge/Platform-x86_64-lightgrey)
  ![Status: Active](https://img.shields.io/badge/Status-Active-brightgreen)
  ![GitHub all releases](https://img.shields.io/github/downloads/boreddevnl/BoredOS/total?color=brightgreen)

  <br />

  [Docs](https://github.com/BoredOS/BoredOS/blob/main/docs/README.md) · [Build & Run](https://github.com/BoredOS/BoredOS/blob/main/docs/build/usage.md) · [AppDev SDK](https://github.com/BoredOS/BoredOS/blob/main/docs/appdev/custom_apps.md) · [Discord](https://discord.gg/J2BxWaFAgY) · [Support](https://buymeacoffee.com/boreddevhq)

</div>

---

![Screenshot](https://raw.githubusercontent.com/BoredOS/BoredOS/refs/heads/main/branding/screenshot.jpg)

> [!NOTE]
> The screenshot above may represent a previous build and is subject to change as the UI evolves.

---

## Features

### Kernel and Architecture
- **Long Mode (x86_64)** 
- **SMP** — Multi-core with IPI-based scheduling and cross-core synchronization
- **Memory Management** — Slab allocator with object pooling; handles physical/virtual mapping
- **VFS** — Unified interface over FAT32, TAR, ProcFS, and SysFS
- **Preemptive Scheduling** — Priority-based, with full context isolation per process
- **Hardware Support** — PCI, AHCI, PS/2, ACPI drivers
- **Virtual Terminals** — 10 independent TTYs (`/dev/tty1`–`/dev/tty10`), each with its own graphics buffer

### Display & Compositing
- **Nova Compositor** — Userland window server over a UNIX socket (`/tmp/nova.sock`)
- **Framebuffer** — `/dev/fb0` for direct pixel access and mode switching
- **Window Management** — Layered rendering, decorations, focus, and client event routing
- **Input Routing** — Keyboard and mouse via `/dev/keyboard` and `/dev/mouse`

### Networking
- **TCP/IP** — lwIP stack with DHCP, DNS, and Berkeley sockets
- **Utilities** — `ping`, `curl`, `telnet`

### Applications
| Category | Applications |
|----------|--------------|
| Shell & CLI | bsh, kilo, ls, grep, find, tar |
| Development | TCC, Lua, POSIX syscalls, custom app framework |
| System | ps, fdisk, mkfs_fat, df, du, lsblk, pci_list, meminfo, sysfetch |
| Graphics | Nova compositor + example clients (taskbar, wallpaper daemon) |
| Network | ping, curl, telnet |


---



## 📚 Documentation

| Guide | Description |
|-------|-------------|
| [Documentation Index](https://github.com/BoredOS/BoredOS/blob/main/docs/README.md) | Start here! |
| [Architecture Overview](https://github.com/BoredOS/BoredOS/blob/main/docs/architecture/README.md) | Deep dive into the kernel |
| [Building and Running](https://github.com/BoredOS/BoredOS/blob/main/docs/build/usage.md) | Set up your build environment |
| [AppDev SDK](https://github.com/BoredOS/BoredOS/blob/main/docs/appdev/custom_apps.md) | Build your own apps for BoredOS |
