# 🐧 LumenFix

**A community-driven Linux utility and GTK control center for automated driver installation, system patching, and GPU management (Nvidia & AMD).**

## 🚀 Overview

LumenFix is a system maintenance utility for Linux environments. Built natively in C++ and GTK, it provides two primary functions: 
1. **Bug Tracker:** A feed that notifies users of recently discovered system issues and vulnerabilities.
2. **Patching Engine:** A centralized hub that delivers temporary, community-verified scripts to address bugs until official upstream updates are released.

Additionally, LumenFix serves as a unified hardware dashboard. It provides telemetry, tuning, automated driver installation, and patch management for both **Nvidia and AMD GPUs** from a single interface, reducing the need to rely on fragmented manufacturer-specific tools.

To ensure compatibility, LumenFix includes **automated distro-detection**. Upon launch, it identifies the host Linux distribution (e.g., Ubuntu, Arch, Fedora) and routes the machine to the community server designated for that specific OS.

## ✨ Key Features

* **Automated Driver Installation:** For distributions that do not include proprietary drivers by default, LumenFix detects the system's hardware and automates the installation of the appropriate Nvidia or AMD drivers, minimizing manual configuration.
* **GPU Telemetry & Control:** Monitor hardware thermals, power draw, and clock speeds for both Nvidia and AMD graphics cards. Apply community-tested driver patches directly through the interface.
* **OS Detection & Routing:** Automatically detects the current Linux distribution and connects the system to the relevant OS-specific server node without requiring user configuration.
* **Community Patching:** Access and apply temporary scripts rolled out by the community to mitigate system instabilities and known bugs.
* **Bug Feed & Alerts:** Receive push notifications when a bug or vulnerability relevant to the user's specific hardware and OS setup is verified by the community.
* **Automated System Analysis:** A background service that monitors hardware and system states, cross-referencing the current configuration with the distro-specific database to suggest relevant available fixes.

## 🏗️ Architecture & Tech Stack

To manage system-level changes securely, LumenFix utilizes a Client-Daemon architecture:
* **Core Language:** C++ (Standard 20+)
* **GUI Frontend (Client):** GTK4 & libadwaita (Wayland-ready)
* **Backend Service (Daemon):** A systemd-managed background service running with elevated privileges to safely execute patches and hardware tuning.
* **Inter-Process Communication (IPC):** D-Bus for secure communication between the GTK UI and the background daemon.
* **Build System:** CMake

## 🚦 Getting Started

**1. Clone the repository:**
```bash
git clone [https://github.com/bogdancoste/LumenFix.git](https://github.com/bogdancoste/LumenFix.git)
cd LumenFix
