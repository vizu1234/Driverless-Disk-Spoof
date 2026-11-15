# 🛡️ Driverless-Disk-Spoof (Decrypted Batch Edition)

> **⚠️ CRITICAL NOTICE:** This tool operates **completely without drivers** (Driverless). It **completely removes** disk serial identifiers rather than nulling them, and all changes are **temporary**—reverting automatically upon system restart.

---

## Overview

A fully decrypted Windows batch script designed to strip disk serial numbers during an active system session. Because it operates entirely in runtime memory without kernel drivers or persistent firmware modifications, restarting your PC completely restores your original hardware identifiers.

---

## Key Features

* **⚡ 100% Driverless:** Requires no kernel-level drivers, vulnerable certificates, or complex loaders.
* **🎯 Complete Serial Removal:** Strips and unlinks serial strings entirely instead of replacing them with null values or placeholders.
* **⏱️ Temporary Session Scope:** Active only during the current boot cycle; fully resets upon reboot.
* **🔓 Fully Decrypted Batch:** Open-source, unencrypted Windows Batch (`.bat`) script for complete code transparency and safety auditing.

---

## System Requirements

* **Operating System:** Windows 10 / Windows 11 (`x64`)
* **Permissions:** Administrator privileges (`cmd.exe`)

---

## Usage Guide

1. Disable third-party antivirus or Windows Defender real-time protection to prevent false-positive quarantines.
2. Place the batch script into a local working directory.
3. Right-click the script and select **Run as Administrator**.
4. Follow the prompt to clear active session serials.
5. **Reboot your PC** when finished to restore default system settings.

---

## Disclaimer

Shared for educational and research purposes only. The user assumes full responsibility for any consequences arising from use.
