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

*   **Every firmware up to 13.60 is jailbreakable depending on your firmware some features such as fpkg support are still being developed for newer firmwares

## 🌐 Web Exploits & Entry Points

Browser environments, network stack mutations, and hosting utilities used to secure userland code execution.

*   **[BD-JB Host Core](https://github.com/Gezine/BD-JB5)** - Blu-ray Disc Java sandbox escape scripts utilized to kickstart code execution on disc-drive equipped hardware.
*   **[PPPwn PS5 Port](https://github.com)** - A network-based PPPoE exploit configuration that targets memory corruption inside the console's network stack.
*   **[UMTX WebKit Implementation](https://github.com)** - [PLACEHOLDER] Front-end browser scripts configured to trigger the UMTX kernel vulnerability on firmwares up to 7.61.

---

## 🚀 Payloads

Post-exploit software binaries that escape app sandboxes, patch system functions, or establish local listeners.

*   **[ETAHEN](https://github.com/etaHEN/etaHEN)** - The standard homebrew enabler for the platform, bundling an integrated FTP engine, plugin systems, and cheat managers.
*   **[PS5-kStuff](https://github.com)** - A kernel-level patch implementation used to authorize the execution of unsigned fPBR files.
*   **[itsPLK Payload Manager](https://github.com)** - A easy to use payload launcher capable of launching .elf and bins for supported ps5s

---

## 🎮 Native Homebrew Apps

Applications compiled specifically for the console's operating architecture using community SDK environments.

*   **[HWInfo-PS5](https://github.com)** - Hardware monitor displaying live internal fan cycles, SoC temperatures, and active core clocks.


---

## 🕹️ Emulators

Virtalization platforms optimized to run classic computing architectures natively on modern hardware.

*   **[swordpdf PS5SX PS5 Port]https://github.com/Swordpdf/PS5SX2** - a native port of PCSX2 to PS5 including 6x resolution .iso .chd .zso support patches/widescreen online play and more.
*   **[mihawk-99 RetroArch PS5 Port]https://github.com/mihawk-99/PS5_RetroArch** - Work-in-progress deployment of the modular frontend emulation framework targeting unlocked firmwares.
*   **[ZiZc3 XPSemu Xemu PS5 Port]https://github.com/ZiZc3/XPSemu** - a original xbox emulator native on ps5.
*   **blackbearreloaded Eden PS5 Port]https://github.com/blackbearreloaded/ProsperoEden** - A switch emulator native on ps5 resolution settings, mods, and more.
*   **[elripalda Dolphin PS5 Port]https://github.com/elripalda/Porpoise-Dolphin-Emulator-for-PS5** - A wii and gamecube emulator native on the PS5 up to 4x resolution, mods, and more
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
