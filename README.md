# DUMP - TOOLS

A Python-based toolkit for Termux (64-bit devices only).

## 📋 Features
- Auto git pull on startup if changes detected
- 64-bit device detection
- Integrated `newd` module for advanced functionality
- Proper error handling and user feedback

## 📁 Files in Repository
- **FILE** - Main executable script
- **newd.cpython-313-aarch64-linux-android.so** - Native module (64-bit ARM)
- **README.md** - This file

## 🚀 Installation & Usage

### Prerequisites
- Termux app
- Python 3.13
- 64-bit Android device

### Quick Start

#### Method 1: Direct Execution
```bash
cd ~/DUMP
chmod +x FILE
./FILE
```

#### Method 2: Python
```bash
cd ~/DUMP
python3 FILE
```

#### Method 3: Full Path
```bash
/data/data/com.termux/files/home/DUMP/FILE
```

## ⚠️ System Requirements
- **Architecture:** 64-bit ARM (aarch64) only
- **Python Version:** 3.13+
- **Device:** 64-bit Android with Termux

### Not Supported
- 32-bit devices will show: `TOOL NOT AVAILABLE FOR 32 BIT DEVICE`

## 🔧 How It Works
1. Detects system architecture (32-bit vs 64-bit)
2. Checks for git changes and auto-updates
3. Sets executable permissions on files
4. Imports and runs the `newd` module on 64-bit devices
5. Provides error messages if module import fails

## 📝 Notes
- The `newd` module is a compiled native extension for Python 3.13
- Ensure both FILE and newd.cpython-313-aarch64-linux-android.so are in the same directory
- Make sure the FILE has execute permissions