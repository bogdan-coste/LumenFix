# 🐧 LumenFix

**An intelligent, community-driven Linux utility and GTK control center offering proactive system patching, universal GPU management (Nvidia & AMD), and auto-configured stability management.**

## 🚀 Overview

LumenFix is designed to be the ultimate safety net and intelligence hub for Linux users. Built natively in C++ and GTK to strictly follow Linux design paradigms, it operates with a powerful **dual-purpose architecture**: 
1. **Intelligence Feed:** A real-time bug tracker that notifies users of newly discovered system issues.
2. **Proactive Patching Engine:** A centralized hub that delivers temporary, community-verified scripts to preempt or fix those bugs until official upstream updates are released.

Beyond OS-level stability, LumenFix serves as a unified hardware dashboard. By bridging the gap between fragmented open-source drivers and proprietary tools, it offers seamless telemetry, tuning, and patch management for both **Nvidia and AMD GPUs** from a single, polished interface.

To ensure flawless compatibility, LumenFix features **automated distro-detection**. Upon launch, it instantly fingerprints your specific Linux distribution (e.g., Ubuntu, Arch, Fedora) and automatically routes your machine to the dedicated community server tailored for that exact OS ecosystem.

## ✨ Key Features

* **Universal GPU Telemetry & Control:** Whether you are on Team Green (Nvidia) or Team Red (AMD), monitor your hardware's thermals, power draw, and clock speeds. Apply community-tested driver patches without relying on clunky, manufacturer-specific software.
* **Smart OS Detection & Routing:** Zero configuration required. LumenFix automatically detects your current Linux distribution and instantly links your system to the dedicated server node for your specific OS architecture.
* **Proactive Community Patching:** When bugs are discovered in your distro's ecosystem, the community rolls out temporary scripts and patches. LumenFix applies these fixes to preempt future crashes or system instabilities before they impact your workflow.
* **Real-Time Bug Feed & Alerts:** Stay ahead of system issues with a built-in news feed. LumenFix sends push notifications the moment a valid bug or vulnerability is verified by the community for your specific setup.
* **AI-Powered System Monitor:** An intelligent background service that continuously analyzes your hardware and system state. It cross-references your configuration with the distro-specific database to suggest only the most relevant fixes.
* **Native Linux Architecture:** Engineered in C++ utilizing GTK and open-source components. LumenFix abandons cross-platform wrappers in favor of a native, lightweight, and visually polished User Experience (UX).

## 🛠️ Tech Stack & Architecture

* **Core Language:** C++
* **GUI Framework:** GTK (Native Linux paradigm)
* **Key Integrations:** Automated Distro Routing, AI System Analysis, Real-time Community Database
* **Target Environment:** Linux Desktop Environments (Cross-Distro, Nvidia & AMD Support)

## 🚦 Getting Started

**1. Clone the repository:**
```bash
git clone [https://github.com/bogdancoste/LumenFix.git](https://github.com/bogdancoste/LumenFix.git)
