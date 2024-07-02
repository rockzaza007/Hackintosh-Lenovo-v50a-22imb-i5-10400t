# Lenovo V50a 22IMB Hackintosh EFI

This repository contains the EFI folder for the Lenovo V50a 22IMB All-in-One PC with an Intel Core i5-10400T processor. The following hardware components are working with this EFI setup:

## Working Components
- ✅ HDMI
- ✅ All USB Ports
- ✅ LAN
- ✅ WiFi + Bluetooth
- ✅ Camera
- ✅ Microphone + Audio

## Not Working
- ❌ AirDrop
- ❌ Touch Screen

## Requirements
- A USB drive with at least 16GB of space
- A copy of macOS (preferably the latest version)
- Basic knowledge of Hackintosh and EFI

## Installation Guide
1. **Prepare the USB drive:**
   - Format the USB drive using Disk Utility.
   - Set the format to `Mac OS Extended (Journaled)`.
   - Set the scheme to `GUID Partition Map`.

2. **Create macOS Installer:**
   - Download macOS from the App Store.
   - Use the terminal command to create the installer:
     ```bash
     sudo /Applications/Install\ macOS\ [version].app/Contents/Resources/createinstallmedia --volume /Volumes/MyVolume
     ```
   
3. **Copy EFI Folder:**
   - Mount the EFI partition of the USB drive.
   - Replace the EFI folder on the USB drive with the EFI folder from this repository.

4. **BIOS Settings:**
   - Disable Secure Boot.
   - Set SATA mode to AHCI.
   - Enable USB Boot.
   - Enable UEFI Boot.

5. **Boot macOS Installer:**
   - Boot from the USB drive.
   - Select the macOS installer in the OpenCore boot menu.
   - Follow the on-screen instructions to install macOS.

6. **Post-Installation:**
   - After installation, boot into macOS from the USB drive again.
   - Mount the EFI partition of your macOS drive.
   - Copy the EFI folder from the USB drive to the EFI partition of your macOS drive.
   - Reboot your system.

## Known Issues
- AirDrop is not working. This is a common issue with many Hackintosh setups.

## Credits
- [OpenCore Team](https://github.com/acidanthera/OpenCorePkg)
- [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
- [Lilu](https://github.com/acidanthera/Lilu)
- [AppleALC](https://github.com/acidanthera/AppleALC)
- [IntelMausi](https://github.com/acidanthera/IntelMausi)
- [AirportItlwm](https://github.com/OpenIntelWireless/itlwm)
- [HACKINTOSH-COMMUNITY](https://github.com/Hackintosh-Community)

## Disclaimer
This EFI folder is provided as-is without any guarantees. Use at your own risk. Make sure to backup your data before attempting to install macOS on your Lenovo V50a 22IMB.
