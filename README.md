# 🐧 LumenFix

**An intelligent, community-driven Linux utility and GTK control center offering automated driver installation, proactive system patching, and universal GPU management (Nvidia & AMD).**

## 🚀 Overview

LumenFix is designed to be the ultimate safety net and intelligence hub for Linux users. Built natively in C++ and GTK to strictly follow Linux design paradigms, it operates with a powerful **dual-purpose architecture**: 
1. **Intelligence Feed:** A real-time bug tracker that notifies users of newly discovered system issues.
2. **Proactive Patching Engine:** A centralized hub that delivers temporary, community-verified scripts to preempt or fix those bugs until official upstream updates are released.

Beyond OS-level stability, LumenFix serves as a unified hardware dashboard. By bridging the gap between fragmented open-source drivers and proprietary tools, it offers seamless telemetry, tuning, automated driver installation, and patch management for both **Nvidia and AMD GPUs** from a single, polished interface.

To ensure flawless compatibility, LumenFix features **automated distro-detection**. Upon launch, it instantly fingerprints your specific Linux distribution (e.g., Ubuntu, Arch, Fedora) and automatically routes your machine to the dedicated community server tailored for that exact OS ecosystem.

## ✨ Key Features

* **Zero-Touch Driver Installation:** For distributions that don't ship with proprietary or up-to-date drivers out of the box, LumenFix automates the entire setup. It detects your hardware and seamlessly installs the correct Nvidia or AMD drivers, saving you from complex manual terminal configurations.
* **Universal GPU Telemetry & Control:** Whether you are on Team Green (Nvidia) or Team Red (AMD), monitor your hardware's thermals, power draw, and clock speeds. Apply community-tested driver patches without relying on clunky, manufacturer-specific software.
* **Smart OS Detection & Routing:** Zero configuration required. LumenFix automatically detects your current Linux distribution and instantly links your system to the dedicated server node for your OS architecture.
* **Proactive Community Patching:** When bugs are discovered in your distro's ecosystem, the community rolls out temporary scripts. LumenFix applies these fixes to preempt future crashes before they impact your workflow.
* **Real-Time Bug Feed & Alerts:** Stay ahead of system issues with a built-in news feed. LumenFix sends push notifications the moment a valid bug or vulnerability is verified by the community for your specific setup.
* **AI-Powered System Monitor:** An intelligent background service that continuously analyzes your hardware and system state. It cross-references your configuration with the distro-specific database to suggest only the most relevant fixes.

## 🏗️ Architecture & Tech Stack

To securely manage system-level changes, LumenFix utilizes a modern Linux Client-Daemon architecture:
* **Core Language:** C++ (Standard 20+)
* **GUI Frontend (Client):** GTK4 & libadwaita (Native Linux paradigm, Wayland-ready)
* **Backend Service (Daemon):** A systemd-managed background service running with elevated privileges to execute patches and hardware tuning securely.
* **Inter-Process Communication (IPC):** D-Bus for secure communication between the GTK UI and the background daemon.
* **Build System:** CMake

## 🚦 Getting Started

**1. Clone the repository:**
```bash
git clone [https://github.com/bogdancoste/LumenFix.git](https://github.com/bogdancoste/LumenFix.git)
cd LumenFix
