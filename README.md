# Ultimate Windows 11 Fresh Install

Personal Windows 11 reinstall checklist.

## 0. Before Installing

- [ ] Back up important files
- [ ] Back up browser data
- [ ] Back up game saves/configs
- [ ] Back up OBS profiles/scenes
- [ ] Back up AutoHotkey scripts
- [ ] Back up Prism Launcher / Minecraft instances
- [ ] Back up any other application configs
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
6. Run Chris Titus Tech WinUtil for the few extra tweaks/tools wanted
   - https://github.com/ChrisTitusTech/winutil
   - Run PowerShell / Terminal **as Administrator**:
     ```powershell
     irm https://christitus.com/win | iex
     ```
7. Run O&O ShutUp10++ for the few additional settings wanted
   - https://www.oo-software.com/en/shutup10
8. Run Remove Windows AI
   - https://github.com/zoicware/RemoveWindowsAI
9. Install legacy/classic Windows tools through Remove Windows AI
10. Apply remaining personal/manual Windows tweaks

## 3. Drivers

- AMD Chipset Software
  - https://www.amd.com/en/support/download/drivers.html
- AMD Radeon Software / Adrenalin
  - https://www.amd.com/en/support/download/drivers.html
- NVIDIA GeForce Driver
  - https://www.nvidia.com/en-us/drivers/
- Motherboard LAN / Wi-Fi / Bluetooth drivers
- Motherboard audio drivers
- Other device-specific drivers
- BIOS/UEFI update if actually needed

## 4. Compatibility / Runtime Packages

### Microsoft Visual C++ Redistributables

- Visual C++ Redistributable Runtimes All-in-One
  - https://www.techpowerup.com/download/visual-c-redistributable-runtime-package-all-in-one/
- Microsoft official latest VC++ Redistributables
  - https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist

### DirectX

- DirectX End-User Runtimes (June 2010)
  - https://www.microsoft.com/en-us/download/details.aspx?id=8109

### .NET

- .NET Framework 3.5
  - https://learn.microsoft.com/en-us/dotnet/framework/install/dotnet-35-windows-11
- Latest .NET Desktop Runtime
  - https://dotnet.microsoft.com/en-us/download/dotnet
- Install both **x64 and x86** Desktop Runtime where applicable

### XNA

- Microsoft XNA Framework Redistributable 4.0 Refresh
  - https://www.microsoft.com/en-us/download/details.aspx?id=27598

### PhysX

- NVIDIA PhysX System Software
  - https://www.nvidia.com/en-us/drivers/physx/physx-system-software/

## 5. Applications

1. 7-Zip
   - https://www.7-zip.org/
2. AMD Chipset Software
   - https://www.amd.com/en/support/download/drivers.html
3. AutoHotkey v2
   - https://www.autohotkey.com/
4. BetterTroveTools
   - https://github.com/AallynReed/BetterTroveTools/releases
5. Discord
   - https://discord.com/download
6. HandBrake
   - https://handbrake.fr/downloads.php
7. Logitech G HUB
   - https://www.logitechg.com/en-us/software/g-hub
8. Mem Reduct
   - https://github.com/henrypp/memreduct
9. Mozilla Firefox
   - https://www.mozilla.org/firefox/new/
10. Notepad++
   - https://notepad-plus-plus.org/downloads/
11. Ninite
   - https://ninite.com/
12. OBS Studio
   - https://obsproject.com/download
13. Prism Launcher
   - https://prismlauncher.org/download/windows/
14. qBittorrent
   - https://www.qbittorrent.org/download
15. r2modman
   - https://thunderstore.io/c/lethal-company/p/ebkr/r2modman/
16. Redragon K673RGB-PRO software
   - https://www.redragonshop.com/
17. Revo Uninstaller
   - https://www.revouninstaller.com/products/revo-uninstaller-free/
18. Steam
   - https://store.steampowered.com/about/
19. SteelSeries GG
   - https://steelseries.com/gg
20. TranslucentTB
   - https://github.com/TranslucentTB/TranslucentTB/releases
21. Vencord
   - https://vencord.dev/download
22. Vocaster Hub
   - https://downloads.focusrite.com/focusrite/vocaster/vocaster-hub
23. LosslessCut
   - https://github.com/mifi/lossless-cut/releases

## 6. Development / General Utilities

- Git
  - https://git-scm.com/download/win
- Python
  - https://www.python.org/downloads/windows/
- Java
  - https://adoptium.net/temurin/releases/
- Java versions required by specific Minecraft versions / projects
- Any additional runtimes or SDKs actually needed

## 7. Ninite

Use Ninite for the standard utilities wanted on a fresh install.

- https://ninite.com/

Keep/use as needed:
- Firefox
- 7-Zip
- Java
- Python
- Other selected utilities

## 8. Final

1. Reboot
2. Make sure all preferred drivers are installed
3. Make sure preferred Windows settings are correct
4. Make sure all preferred applications are installed
5. Restore personal files/configs
6. Restore game saves / profiles / scripts
7. Done
