# iOS Disable Call Recording (Books Exploit)

![Badge](https://img.shields.io/badge/iOS-26--26.1-blue)
![Badge](https://img.shields.io/badge/Status-Stable-brightgreen)
![Badge](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS-lightgrey)
![Badge](https://img.shields.io/badge/Author-YangJiii-orange)

A tool that replaces or disables the call‑recording notification sound
(Start/Stop Disclosure) on iOS **without Jailbreak**, using the **Books
app file‑overwrite exploit**.

Supports **iOS 26.0 → iOS 26.1**

**Author:** YangJiii --- @duongduong0908\
**Original Developer:** Huy Nguyen --- @Little_34306

------------------------------------------------------------------------

## ⚠️ DISCLAIMER & LEGAL NOTICE

Before using this tool, you **MUST** read and agree to all of the
following terms:

------------------------------------------------------------------------

## 1. Device & Data Risk

-   This tool modifies internal iOS files using a security
    vulnerability.\
-   There is always a risk of device issues (boot loop, soft brick, data
    loss).\
-   **The author (YangJiii) takes NO responsibility** for any hardware
    damage, software corruption, or data loss.\
-   You use this tool entirely **at your own risk**.

------------------------------------------------------------------------

## 2. Legal Notice About Call Recording

-   The "StartDisclosure" sound exists to comply with privacy laws in
    many countries.\
-   Removing or silencing this sound **may violate privacy or
    eavesdropping laws** depending on your region.\
-   This tool is for **educational research only**.\
-   The author is **not responsible** for any misuse.

------------------------------------------------------------------------

# 📂 Required Folder Structure

Before running the tool, ensure your files are arranged like this:

    Your_Tool_Folder/
    │
    ├── windows.py
    ├── mac.py
    ├── uuid.txt
    │
    └── Sounds/
        ├── StartDisclosureWithTone.m4a
        └── StopDisclosure.m4a

------------------------------------------------------------------------

# 💻 WINDOWS GUIDE

## STEP 1 --- INSTALL REQUIRED COMPONENTS

### 1. Install iTunes

Download from Apple's website.\
Ensure iTunes detects your iPhone.

### 2. Install Python

Download from: https://python.org\
✔️ Select **Add Python to PATH**.

### 3. Install Libraries

    pip install PyQt5 pymobiledevice3 click requests packaging

------------------------------------------------------------------------

## 🔧 Additional Fix for pymobiledevice3 Installation (Windows Only)

If installing `pymobiledevice3` causes build errors, you must install
the required C++ components.

### ✔️ 1. Install Microsoft Visual C++ Build Tools

Download:\
https://visualstudio.microsoft.com/visual-cpp-build-tools/

Select during installation: - Desktop development with C++ - MSVC
v143+ - Windows 10/11 SDK

Restart after installation.

### ✔️ 2. Install Microsoft Visual C++ Redistributable 2015--2022

x64: https://aka.ms/vs/17/release/vc_redist.x64.exe\
x86: https://aka.ms/vs/17/release/vc_redist.x86.exe

Install both → Restart.

### ✔️ Reinstall pymobiledevice3

    pip install pymobiledevice3

------------------------------------------------------------------------

## 🚀 STEP 2 --- RUN THE TOOL

Run CMD as Administrator:

    python windows.py

------------------------------------------------------------------------

# 🍎 MACOS GUIDE

## STEP 1 --- INSTALL LIBRARIES

    pip3 install PyQt5 pymobiledevice3 click requests packaging

## STEP 2 --- RUN THE TOOL

    python3 mac.py

------------------------------------------------------------------------

# ❓ COMMON ISSUES & FIXES

### 1. No device found

-   Check iTunes (Windows)
-   Press **Trust** on iPhone

### 2. Timeout

-   Same Wi-Fi network required\
-   Disable Windows Firewall

### 3. UUID not found

Open **Books** → download a book → try again.

### 4. WinError 1231

Network issue → toggle Wi‑Fi.

------------------------------------------------------------------------

## ☕ Support

If this project helped you, consider supporting via **Ko-fi** ❤️\
👉 https://ko-fi.com/yangjiii/goal?g=1
