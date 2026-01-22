# Android 16KB Page Size Alignment Checker

Command-line tool to verify **16KB ELF alignment compliance** for Android native libraries.

Google Play requires apps targeting Android 15+ (Nov 2025) to support 16KB page sizes.  
This script scans APKs or `.so` files and reports which libraries must be rebuilt.

---

## Features
- Works with APK, APEX, or library folders
- Detects ELF alignment using objdump
- PASS / FAIL summary
- No Android Studio required
- CI/CD friendly

---

## Supported OS
- Linux
- macOS
- (Windows via WSL only)

---

## Requirements
- bash
- objdump
- unzip
- file
- zipalign (optional)

---

## Usage
```bash
bash check_alignment.sh app-release.apk
