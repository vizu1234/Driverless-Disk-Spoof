# Driverless-Disk-Spoof (Decrypted Batch Edition)

---

## Overview

This repository hosts the **Driverless-Disk-Spoof**, a fully decrypted Windows batch script designed to strip and clear disk serial identifiers during an active operating system session. 

> [!NOTE]
> **Important Operating Behavior:** This is a **temporary (session-based)** spoof. The modifications applied by this script exist only within the current running state of the operating system and **revert automatically once you restart your computer**. 

Unlike permanent flashing methods that alter physical firmware or NVRAM storage blocks, this script interacts with runtime device properties and active system handles. Because these identifiers are dynamically regenerated or re-enumerated by the Windows Plug and Play (PnP) manager upon boot, a system restart restores the default hardware serial numbers.

---

## Technical Mechanics & How It Works

1. **Runtime Property Stripping:** The script executes native command-line utilities (`cmd`, `wmic`, or registry queries depending on the script's specific implementation structure) to target active storage controller paths and physical disk identifiers.
2. **Volatile State Modification:** By clearing or unlinking the serial strings from the active device tree during runtime, applications or services querying WMI (Windows Management Instrumentation) or storage device properties during the current session fail to retrieve valid hardware strings.
3. **Session Lifecycle:** Because the modifications are applied to the active OS kernel/device registry state without modifying the underlying disk firmware, restarting the system forces Windows to re-query the physical hardware, cleanly rebuilding the original serial numbers.

---

## Features

* **Native Batch Architecture:** Built entirely in standard Windows Batch (`.bat`), requiring no external compiler, runtime environment, or third-party dependencies.
* **Fully Decrypted & Auditable:** Zero obfuscation or encryption. Every command and execution loop can be inspected directly in any text editor.
* **Session-Based Action:** Operates entirely within the current boot cycle, ensuring that standard hardware parameters are safely restored upon the next system reboot.
* **Direct Identifier Targeting:** Focuses specifically on removing disk serial strings rather than leaving static null placeholders.

---

## System Requirements

| Component | Requirement |
| :--- | :--- |
| **Operating System** | Windows 10 / Windows 11 (`x64` architecture) |
| **Permissions** | Full Administrator privileges |
| **Environment** | Standard Windows Command Prompt (`cmd.exe`) |

---

## Step-by-Step Usage Guide

> [!IMPORTANT]
> **Pre-requisite:** Before executing the script, ensure that Windows Defender real-time protection or any third-party antivirus software is temporarily disabled. Low-level storage and registry modification scripts routinely trigger heuristic false positives.

### 1. Preparation
Place the script file into a local working directory on your primary drive. Do not run the script directly from inside a compressed archive or temporary extraction folder.

### 2. Administrator Execution
Right-click the batch file and select **Run as Administrator**. Administrative rights are required to interact with system-level device spaces and storage queries.

### 3. Execution
Allow the script to process the target disk identifiers. Review the command-line feedback output to confirm successful execution.

### 4. Session Persistence Note
Keep in mind that these changes remain active **only until your next system reboot**. If you shut down or restart your computer, you will need to re-run the script if you require the spoof to be active for the new session.

---

## Troubleshooting & FAQ

* **Q: Do I need to run this every time I turn on my PC?**
  * **A:** Yes. Because this is a temporary session spoof, restarting your computer clears the modified runtime state and reloads your original hardware serial numbers from the physical disk firmware.
* **Q: The script terminates immediately or returns access denied errors.**
  * **A:** Ensure you are launching the script with full administrator rights and that your antivirus software has not quarantined or blocked the execution process.

---

## Disclaimer & Credits

* **Developer:** `vizu1234` (GitHub)
* **Disclaimer:** This software and its contents are provided strictly for educational, informational, and research purposes. The user assumes full responsibility for any consequences arising from the execution or usage of this script.
