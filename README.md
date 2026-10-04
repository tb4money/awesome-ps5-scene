# Awesome PS5 Homebrew & Scene [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

> A curated collection of working PlayStation 5 (PS5) homebrew projects, exploit implementations, payloads, emulators, and low-level development utilities.

This repository catalogs open-source projects, reverse-engineering documentation, and software environments built by the console scene. 

⚠️ **Strict Anti-Piracy Policy:** This list is strictly dedicated to homebrew creation, system security research, and custom emulation layers. Links to commercial game backups, cracked security keys, or illicit distribution channels are strictly prohibited and will be rejected immediately.

---

## 📑 Contents

- [Firmware & Exploit Status](#-firmware--exploit-status)
- [Web Exploits & Entry Points](#-web-exploits--entry-points)
- [Kernel Exploits & Payloads](#-kernel-exploits--payloads)
- [Native Homebrew Apps](#-native-homebrew-apps)
- [Emulators](#-emulators)
- [Alternative OS & Linux](#-alternative-os--linux)
- [PC & Development Tools](#-pc--development-tools)
- [Hardware Interfacing & UART](#-hardware-interfacing--uart)
- [Research Documentation](#-research-documentation)
- [Scene Resources & News](#-scene-resources--news)

---

## 🔑 Firmware & Exploit Status

Console security states are defined entirely by your system firmware revision. If you want to run custom code, keep your system completely offline and do not update.

*   **Firmwares 1.00 - 2.50** — Vintage launch-era software. Highly sought after for low-level architecture mapping and hypervisor vulnerability research.
*   **Firmwares 3.00 - 4.51** — The definitive homebrew target. Native compatibility with the WebKit/BD-J userland entry points paired with the IPV6 kernel exploit. Full write access to system memory via stable payload environments.
*   **Firmwares 5.00 - 7.61** — The UMTX vulnerability threshold. These firmwares leverage the `bypervisor` implementation of the UMTX kernel exploit via the WebKit userland. Offers kernel read/write primitives, though hypervisor constraints remain active.
*   **Firmwares 8.00 - 9.60** — Userland access limits. Vulnerable to the `PPPwn` PPPoE network stack exploit and specific WebKit entry points, but lacking a public, stable kernel-level execution chain.
*   **Firmwares 10.00+** — Patched territory. Safe from all known public software entry points. 

---

## 🌐 Web Exploits & Entry Points

Browser environments, network stack mutations, and hosting utilities used to secure userland code execution.

*   **[BD-JB Host Core](https://github.com)** - Blu-ray Disc Java sandbox escape scripts utilized to kickstart code execution on disc-drive equipped hardware.
*   **[PPPwn PS5 Port](https://github.com)** - A network-based PPPoE exploit configuration that targets memory corruption inside the console's network stack.
*   **[UMTX WebKit Implementation](https://github.com)** - [PLACEHOLDER] Front-end browser scripts configured to trigger the UMTX kernel vulnerability on firmwares up to 7.61.

---

## 🚀 Kernel Exploits & Payloads

Post-exploit software binaries that escape app sandboxes, patch system functions, or establish local listeners.

*   **[ETAHEN](https://github.com)** - The standard homebrew enabler for the platform, bundling an integrated FTP engine, plugin systems, and cheat managers.
*   **[Libhijacker](https://github.com)** - Run-time modification framework designed to break out of retail app constraints and sustain active background execution threads.
*   **[PS5-kStuff](https://github.com)** - A kernel-level patch implementation used to authorize the execution of unsigned fPBR files.
*   **[PS5-Payload-ElfLoader](https://github.com)** - A local network daemon that maps to an open TCP port on the console, waiting to execute incoming `.elf` payloads.

---

## 🎮 Native Homebrew Apps

Applications compiled specifically for the console's operating architecture using community SDK environments.

*   **[HWInfo-PS5](https://github.com)** - Hardware monitor displaying live internal fan cycles, SoC temperatures, and active core clocks.
*   **[Mast1c0re Network Game Loader](https://github.com)** - Injector client that targets the built-in PS4 backward compatibility layers via manipulated save games.
*   **[PS5 Homebrew Store](https://github.com)** - Graphical storefront interface allowing users to browse, download, and patch community applications directly from the console UI.
*   **[File Manager Placeholder](https://github.com)** - [PLACEHOLDER] A visual shell app built to navigate user directories on the internal `/data` partition.

---

## 🕹️ Emulators

Virtalization platforms optimized to run classic computing architectures natively on modern hardware.

*   **[Mast1c0re PS1/PS2 Layer](https://github.com)** - Practical implementations targeting the console's native, internal PS2 emulation runtime using sandbox bypasses.
*   **[RetroArch PS5 Port](https://github.com)** - Work-in-progress deployment of the modular frontend emulation framework targeting unlocked firmwares.

---

## 💾 Alternative OS & Linux

Custom boot environments, alternative kernels, and hardware-accelerated Linux distributions.

*   **[PS5 Linux Kernel Fork](https://github.com)** - [PLACEHOLDER] Source modifications aiming to map individual hardware targets, including early attempts at custom Southbridge and GPU acceleration.

---

## 🛠️ PC & Development Tools

Desktop compiler toolchains, network utilities, and decompilation resources used to build or parse payload binaries.

*   **[Netcat GUI](https://github.com)** - Minimalist desktop dashboard used to broadcast compiled `.elf` assets to a designated local network IP.
*   **[Prosper0g](https://github.com)** - Official diagnostics and scripts built to read out early firmware structures and configuration layers.
*   **[PS5-Payload-SDK](https://github.com)** - Complete C/C++ development environment built on LLVM/Clang to facilitate native software compilation.

---

## 🔌 Hardware Interfacing & UART

Motherboard revisions, serial communication interfaces, hardware glitching setups, and diagnostic trace methods.

*   **[UART Serial Logging Guide](https://github.com)** - [PLACEHOLDER] Schematic diagrams and console terminal setup steps detailing how to solder to the motherboard's TX/RX contact pads for low-level crash output logs.

---

## 🔮 Research Documentation

In-depth technical write-ups, vulnerability disclosures, and architectural security breakdowns.

*   **[Bypervisor Exploit Notes](https://github.com)** - [PLACEHOLDER] Security write-up detailing the structure of the UMTX kernel vulnerability and its behavior alongside the hypervisor.
*   **[PS5 Hypervisor Disclosures](https://github.com)** - Whitepapers and assembly documentation detailing secure memory structures and privilege levels by fail0verflow.

---

## 🌐 Scene Resources & News

Aggregators and community databases hosting configuration files, step-by-step documentation, and verified release logs.

*   **[PS5 Exploits Interactive Guide](https://moddedintentions.com)** - Step-by-step breakdown used to verify firmware versions and configure safe DNS filtering setups.
*   **[PSX-Place Community Index](https://psx-place.com)** - Active developer forums housing hardware troubleshooting advice, technical logs, and release alerts.
*   **[Wololo.net Blog](https://wololo.net)** - Longstanding platform news portal covering exploit disclosures, developer presentation notes, and open-source updates.

---

## 🤝 Contribute

Contributions are welcome! Please read the [Contribution Guidelines](contributing.md) to inspect our repository structural layout, lint rules, and alphabetical sorting requirements before opening a pull request.

## 📝 License

[![CC0](https://licensebuttons.net)](https://creativecommons.org)

To the extent possible under law, all contributors have waived copyright and related or neighboring rights to this repository under the **CC0-1.0 Universal License**.
