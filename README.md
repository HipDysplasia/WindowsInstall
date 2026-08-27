# Ultimate Windows 11 Fresh Install

Personal Windows 11 reinstall checklist.

## 0. Before Installation

- [ ] Back up important files
- [ ] Back up browser data
- [ ] Back up Discord/Vencord export
- [ ] Back up OBS profiles/scenes
- [ ] Back up AutoHotkey scripts
- [ ] Back up Prism Launcher / Minecraft instances
- [ ] Back up other application configs
- [ ] Prepare Ventoy USB
  - https://www.ventoy.net/en/download.html

## 1. Windows Installation

1. Download a fresh Windows 11 ISO directly from Microsoft
   - https://www.microsoft.com/software-download/windows11
2. Install GParted Live onto the Ventoy USB
   - https://gparted.org/livecd.php
3. BIOS:
   - UEFI: **Enabled**
   - CSM / Legacy: **Disabled**
   - Secure Boot: **Disabled**
   - TPM / fTPM: **Enabled**
4. Boot Ventoy
5. Use GParted to wipe/repartition drives
6. Install **Windows 11 Pro — NOT N**
7. At OOBE:
   - `Shift + F10`
   - `OOBE\BYPASSNRO`
8. Click **No** on optional/privacy prompts
9. Run Windows Update
10. Reboot
11. Run Windows Update again
12. Repeat until there are no updates left

> If `OOBE\BYPASSNRO` is removed/does not work on a future Windows build, update this step.

## 2. Post-Install

1. Install FSOS-X
   - https://fsosx.com/
2. Configure FSOS-X / FSOS-X Dash
3. Install hardware drivers
4. Reboot
5. Apply personal Windows settings/tweaks
6. Run Chris Titus Tech WinUtil for the extra tweaks wanted
   - https://github.com/ChrisTitusTech/winutil
   - Run PowerShell / Terminal **as Administrator**:
     ```powershell
     irm https://christitus.com/win | iex
     ```
7. Run O&O ShutUp10++ for the additional settings wanted
   - https://www.oo-software.com/en/shutup10
8. Run Remove Windows AI
   - https://github.com/zoicware/RemoveWindowsAI
9. Install legacy/classic Windows tools through Remove Windows AI
10. Apply remaining personal/manual Windows tweaks

## 3. Hardware Drivers

### CPU / Chipset

- AMD Ryzen 7 5800X / B550 Chipset
  - https://www.amd.com/en/support/downloads/drivers.html/chipsets/am4/b550.html
- Current AMD Chipset Driver: **8.08.12.551**

### GPU

- Current GPU: **GIGABYTE GeForce RTX 3060 GAMING OC 12G 2.0**
  - https://www.nvidia.com/en-us/drivers/
- If/when replaced with AMD Radeon GPU:
  - https://www.amd.com/en/support/download/drivers.html

### LAN

- Realtek RTL8125 2.5GbE
  - ASUS Windows 11 driver: **1125.27.50.919**
  - https://www.asus.com/pl/motherboards-components/motherboards/tuf-gaming/tuf-gaming-b550-plus/helpdesk_download?model2Name=TUF-GAMING-B550-PLUS

### Audio

- Realtek ALC1200
  - ASUS Windows 11 driver: **6.0.9888.1**
  - https://www.asus.com/pl/motherboards-components/motherboards/tuf-gaming/tuf-gaming-b550-plus/helpdesk_download?model2Name=TUF-GAMING-B550-PLUS

### Wi-Fi / Bluetooth

- **None detected in HWiNFO report**
- No driver required unless a separate adapter is installed

### BIOS / UEFI

- ASUS TUF GAMING B550-PLUS
  - Current BIOS in report: **3621**
  - Latest BIOS currently available: **3644**
  - https://www.asus.com/pl/supportonly/tuf%20gaming%20b550-plus/helpdesk_bios/

## 4. Compatibility / Runtime Packages

### Microsoft Visual C++ Redistributables

- Visual C++ Redistributable Runtimes All-in-One
  - https://www.techpowerup.com/download/visual-c-redistributable-runtime-package-all-in-one/
- Microsoft official latest VC++ Redistributables
  - https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist

> The All-in-One package is for broad legacy compatibility. The official Microsoft package is the current supported v14 runtime.

### DirectX

- DirectX End-User Runtimes (June 2010)
  - https://www.microsoft.com/en-us/download/details.aspx?id=8109

> Windows already contains the modern DirectX runtime. June 2010 provides legacy side-by-side components required by some older games.

### .NET

- .NET Framework 3.5
  - https://learn.microsoft.com/en-us/dotnet/framework/install/dotnet-35-windows-11
- Latest .NET Desktop Runtime
  - https://dotnet.microsoft.com/en-us/download/dotnet/10.0

> Windows 11 already includes .NET Framework 4.8.1. Install additional modern .NET Desktop Runtime versions only as needed.

### XNA

- Microsoft XNA Framework Redistributable 4.0 Refresh
  - https://www.microsoft.com/en-us/download/details.aspx?id=27598

### Optional Legacy Compatibility

- NVIDIA PhysX System Software
  - https://www.nvidia.com/en-us/drivers/physx/physx-system-software/

> Optional. Only install if a specific game/application requires it.

## 5. Applications

1. 7-Zip
2. AMD Chipset Software
3. AutoHotkey v2
4. Better Trove Tools
5. Discord
6. HandBrake
7. Logitech G HUB
8. Mem Reduct
9. Mozilla Firefox
10. Notepad++
11. Ninite
12. OBS Studio
13. Prism Launcher
14. qBittorrent
15. r2modman
16. Redragon K673RGB-PRO
17. Revo Uninstaller
18. Steam
19. SteelSeries GG
20. TranslucentTB
21. Vencord
22. Vocaster Hub
23. LosslessCut

## 6. Ninite

- https://ninite.com/

Use Ninite for the standard utilities wanted on a fresh install.

## 7. Final

1. Reboot
2. Make sure drivers are installed
3. Make sure Windows settings are correct
4. Make sure applications are installed
5. Restore personal files/configs
6. Restore game saves/profiles/scripts
7. Done
