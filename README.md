# Awesome PS5 Homebrew & Scene [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

> A curated list of high-quality PlayStation 5 (PS5) homebrew, exploits, payloads, emulators, and system utilities.

<img src="[![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)" align="
This list focuses strictly on **homebrew development, system diagnostics, and hardware virtualization**. It serves as a comprehensive reference guide for developers and enthusiasts looking to safely interface with the PlayStation 5 ecosystem.

⚠️ **Strict Policy:** Content regarding piracy, commercial game backups, illicit distribution networks, or leaked cryptographic keys is strictly banned and will be immediately rejected.

---

## 🗺️ Navigation Menu

[Contributing Guidelines](contributing.md) • [Code of Conduct](code-of-conduct.md) • [Official Website](https://awesome.re) • [Community Forum](#-resources--communities)

---

## 📑 Contents

- [Firmware & Exploit Status](#-firmware--exploit-status)
- [Payloads & Kernels](#-payloads--kernels)
- [Homebrew Apps](#-homebrew-apps)
- [Emulators](#-emulators)
- [PC & Development Tools](#-pc--development-tools)
- [Upcoming Tools & Research](#-upcoming-tools--research)
- [Resources & Communities](#-resources--communities)

---

## 🔑 Firmware & Exploit Status

A chronological breakdown of vulnerable firmware thresholds, entry points, and active capabilities. Keep your console offline and do not update if you intend to run custom code.

*   **Firmware 1.xx - 2.xx** — Baseline hardware revisions. Highly vulnerable, historically significant for early hypervisor reverse-engineering and native hardware research.
*   **Firmware 3.00 - 4.51** — The active "Golden Era" firmware range. Features full native stability for WebKit and BD-J kernel exploits, providing a robust environment for homebrew frameworks.
*   **Firmware 5.00 - 7.61** — WebKit and IPv6 userland entry points are accessible. Active ongoing research applies kernel exploit implementations (such as `bypervisor`) to these layers.
*   **Firmware 8.00+** — Modern patched territory. No public kernel entry points exist. 

---

## 🚀 Payloads & Kernels

Software designed to escape native application sandboxes, inject custom code, or establish post-exploit execution environments.

*   **[ETAHEN](https://github.com)** - The premier PS5 Homebrew Enabler featuring an integrated FTP server, a cheat engine, and active plugin loading support.
*   **[PS5-kStuff](https://github.com)** - Kernel patch framework allowing the execution of unsigned code and customized homebrew fPBRs.
*   **[PS5-Payload-ElfLoader](https://github.com)** - An ELF payload loader that listens on a dedicated network port to boot code directly onto exploited consoles.
*   **[Libhijacker](https://github.com)** - Advanced utility designed to break out of the PS5 application sandbox and run arbitrary background processes.

---

## 🎮 Homebrew Apps

Applications built natively by the community using open-source toolchains to run directly on your retail hardware.

*   **[PS5 Homebrew Store](https://github.com)** - An on-console graphical package manager used to download, update, and manage community applications over the air.
*   **[Mast1c0re Network Game Loader](https://github.com)** - Bootstraps local network payloads using the PS4 `OKAGE: Shadow King` save-game exploit layer.
*   **[HWInfo-PS5](https://github.com)** - System diagnostic tool displaying live hardware telemetry including fan duty cycles, SoC temperatures, and frequency scaling.

---

## 🕹️ Emulators

Software designed to repurpose native hardware execution layers for retro gaming and system virtualization.

*   **[RetroArch PS5 Port](https://github.com)** - Ongoing development port bringing the universal modular emulation frontend to vulnerable PS5 systems.
*   **[Mast1c0re PS1/PS2 Emulator](https://github.com)** - Utilizes native, built-in backward compatibility layers inside the console to run classic software safely via sandbox escapes.

---

## 🛠️ PC & Development Tools

Desktop software and compilation frameworks required to build payloads, run network utilities, or interface with an exploited console.

*   **[PS5-Payload-SDK](https://github.com)** - A complete, open-source software development kit utilizing LLVM/Clang for compiling custom C/C++ payloads.
*   **[Prosper0g](https://github.com)** - Official diagnostic utility infrastructure scripts used to interact with early system maintenance components.
*   **[Netcat GUI](https://github.com)** - A streamlined desktop application built to broadcast compiled `.elf` payloads to a console's local IP address.

---

## 🔮 Upcoming Tools & Research

Active repositories containing architectural documentation, security papers, and proof-of-concept software updates.

*   **[PS5 Hypervisor Research](https://github.com)** - In-depth architectural analysis and exploit documentation targeting the PS5 secure hypervisor layers by fail0verflow.
*   **[BD-JB Exploitation Core](https://github.com)** - Blu-ray Disc Java sandbox escapes utilized to trigger arbitrary code execution on disc-drive compatible consoles.
*   **[PPPwn PS5 Port](https://github.com)** - Experimental network stack implementation modifying the PPPoE vulnerability to target higher firmware thresholds.

---

## 🌐 Resources & Communities

Centralized knowledge hubs, staging sites, and community forums tracking live developments within the PlayStation scene.

*   **[PS5 Exploits Guide](https://moddedintentions.com)** - The definitive step-by-step documentation guide for safely identifying, configuring, and maintaining low-firmware consoles.
*   **[PSX-Place PS5 Forum](https://psx-place.com)** - Longstanding scene message boards featuring developer logs, community support threads, and hardware troubleshooting.
*   **[Wololo.net](https://wololo.net)** - A news aggregator providing daily updates on cryptographic disclosures, security conferences, and open-source project releases.

---

## 🤝 Contribute

Contributions are highly encouraged! Please review the [Contribution Guidelines](contributing.md) to learn about our repository structure, link formatting rules, and strict quality control standards before opening a pull request.

## 📝 License

[![CC0](https://licensebuttons.net)](https://creativecommons.org)

To the extent possible under law, all contributors have waived copyright and related or neighboring rights to this repository under the **CC0-1.0 Universal License**.
