# Industrial LED Inspection System

Industrial vision inspection system for real-time LED ON/OFF detection using Python, OpenCV, PLC communication, MES integration, SPC dashboard, and secure Operator/Engineer modes.

# Overview

The Industrial LED Inspection System is a Python-based desktop application designed for automated LED inspection in manufacturing environments.

The system captures images from a camera, analyzes configurable Regions of Interest (ROIs), and determines whether each LED is ON or OFF based on brightness, color, and fill percentage. It supports PLC communication for machine integration, optional MES connectivity, SPC dashboards for quality monitoring, and complete audit logging for traceability.

This software was developed to improve inspection accuracy, reduce false NG results, and provide a robust and user-friendly platform for both operators and engineers.

# Key Features

# Vision Inspection
Real-time LED ON/OFF detection
Rectangle and circular ROI support
Brightness, color, and fill-percentage analysis
PASS/FAIL decision logic
Snapshot capture for failed inspections
Auto ROI tools
Debug overlays

# Camera Control
Multi-camera support
Camera scanning and selection
Auto/manual focus
Brightness and zoom control
Watchdog auto-reconnect

# PLC Integration
Delta PLC Modbus TCP communication
Support for D, M, X, and Y devices
Read/write and force controls
PLC Debug Console
Batch write and snapshot export
# MES Integration
Optional proprietary DLL-based MES interface
Standalone mode supported when DLLs are not available
# SPC Dashboard
Yield trend chart
PASS/FAIL pie chart
Fail-by-ROI analysis
LED intensity trend
# User Management
Operator mode
Engineer/Admin mode
Password-protected configuration
Audit trail with user and editor tracking
# Project Management
Save/load/copy project configurations
Automatic backups
Change logs
# Audit and Traceability
Inspection logs
Project edit logs
Snapshot evidence
CSV/Excel/PDF export

# Technology Stack

Python 3
PyQt5
OpenCV
NumPy
pyModbusTCP
pythonnet
Pandas
OpenPyXL

# Project Structure

Industrial-LED-Inspection-System/
├── led_check_app.py
├── README.md
├── LICENSE
├── .gitignore
├── requirements.txt
├── auth.json                # Local credentials (not included)
├── mes/
│   └── dll/                 # Proprietary DLLs (not included)
├── logs/                    # Runtime logs (ignored)
├── result_captures/         # Inspection images (ignored)
└── projects/                # Saved project files (ignored)

# Installation
git clone https://github.com/victory0503/Industrial-LED-Inspection-System.git
cd Industrial-LED-Inspection-System
pip install -r requirements.txt
python led_check_app.py

# Requirements
Python 3.9+
Windows OS
Camera device
Optional Delta PLC
Optional MES DLLs

# Proprietary Components

This repository does not include proprietary MES DLL files or confidential production data.

The following items are intentionally excluded:

DLLFunctionAll.dll
TDC_DLL.dll
auth.json
Production logs
Customer-specific project files

The application can run in standalone mode without MES integration.

# Screenshots

Add screenshots here for:

Main Operator Screen
Engineer Mode
PLC Debug Console
SPC Dashboard
View Log Window

# Business Impact
Reduced false rejects by improving LED detection accuracy
Increased inspection reliability and traceability
Simplified troubleshooting with integrated PLC debugging
Enabled secure separation between operator and engineering functions

# Author

Vorachai Somsuay
Automation Engineer | Python Developer | Industrial Automation Engineer

LinkedIn: https://www.linkedin.com/in/vorachai-somsuay
GitHub: https://github.com/victory0503

# License

This project is licensed under the MIT License. See the LICENSE file for details.
