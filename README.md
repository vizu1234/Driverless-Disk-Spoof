# 🛡️ Driverless-Disk-Spoof (Decrypted Batch Edition)

<p align="center">
  <img src="https://img.shields.io/badge/OS-Windows%2010%20%2F%2011-blue?style=for-the-badge&logo=windows" alt="Windows">
  <img src="https://img.shields.io/badge/Language-Batch%20(.bat)-orange?style=for-the-badge&logo=windows-terminal" alt="Batch">
  <img src="https://img.shields.io/badge/Status-Fully%20Decrypted-success?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/badge/Action-Serial%20Stripping-critical?style=for-the-badge" alt="Action">
</p>

---

## 📌 Overview

This repository hosts the **Driverless-Disk-Spoof**, a fully decrypted, native Windows batch script engineered to completely strip and remove disk serial identifiers at the system level rather than simply nulling them out. 

> [!NOTE]
> This release is completely unencrypted and open for community inspection. It targets disk serial structures directly through native command-line workflows with zero complex setup required.

---

## ✨ Features

*   **⚡ Native Batch Scripting:** Written entirely in lightweight Windows Batch (`.bat`), requiring no external dependencies, runtimes, or compiled binaries.
*   **🔓 Fully Decrypted Source:** Zero obfuscation or encryption. Every command, query, and operation is fully visible and auditable.
*   **🎯 Complete Serial Stripping:** Unlike standard methods that leave placeholder or null values, this tool completely removes disk serial numbers from target drives.
*   **🤖 Lightweight Execution:** Streamlined and fast interface designed for rapid execution and immediate results.

---

## 📋 System Requirements

| Component | Requirement |
| :--- | :--- |
| **Operating System** | Windows 10 / Windows 11 (`x64` architecture) |
| **Permissions** | Full Administrator privileges required |
| **Script Environment** | Native Windows Command Prompt (`cmd.exe`) |

---

## 🚀 Step-by-Step Usage Guide

> [!IMPORTANT]
> **Pre-requisite:** Before running the script, ensure your **Windows Defender** and any third-party antivirus software are disabled. Low-level disk management and query scripts frequently trigger false-positive heuristic flags.

### 1. Extraction / Placement
Place the script file (`.bat`) into a dedicated working folder on your primary drive.

### 2. Execute as Administrator
Right-click the batch script and select **Run as Administrator** to ensure it has the necessary permissions to interact with disk subsystems.

### 3. Execution
Follow the on-screen prompts within the command-line interface to execute the disk serial stripping sequence.

### 4. Reboot
Perform a **complete system restart** immediately after execution to flush the disk cache and ensure changes are registered properly by the OS.

---

## 🛠️ Troubleshooting & FAQ

*   **Q: Do I need special dependencies installed to run this?**
    *   *A:* No. Because it is written entirely in native batch, it runs directly using standard Windows command-line utilities.
*   **Q: The script closes immediately or throws access errors.**
    *   *A:* Make sure you are running the script with full Administrator privileges and that real-time antivirus protection is temporarily disabled.

---

## ⚖️ Disclaimer & Credits

*   **Developer:** `vizu1234` (GitHub)
*   **Disclaimer:** This software and its contents are shared for educational, informational, and archival research purposes only. The user assumes full responsibility for any consequences arising from the usage of this script.
