# Nexus USB HATS

Install and play games from external USB storage on a compatible modified Nintendo Switch.

**Nexus Atmosphere 1.12.2 N3 · Switch firmware 23.5.0 support · Hekate 6.5.5 / Nyx 1.9.5 · Nexus Manager 0.2.16**

[Download the latest release](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/latest) · [What's changed](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/tag/v1.12.2-n3) · [Report a problem](https://github.com/TR4UNEXUS/Nexus-USB-HATS/issues)

Keep a larger game library on an external HDD, SSD or USB flash drive. Your microSD card still holds the console setup and the information that connects your USB library to the system.

## Choose a pack

Both current packs use the **standard Hekate appearance and original Atmosphere splash**, with the Nexus build version and USB support retained. Neither includes the custom Nexus boot theme.

| Pack | Choose it if… |
| --- | --- |
| [**Standard No-HOC**](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-n3/Nexus-1.12.2-N3-Standard-No-HOC.zip) | You want Nexus USB support without HOC's clock controls. |
| [**Standard HOC**](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-n3/Nexus-1.12.2-N3-Standard-HOC.zip) | You also want the included Nexus-compatible HOC 2.6.0 and its overlay. |

Choose **one** pack. Both include Nexus Manager as an NRO and installable NSP, the USB Content overlay with coloured notifications, sys-patch, Nintendo DNS rules, and ready-made Hekate Launch entries.

These are the current standard packs. The older Full and themed packs remain in [previous releases](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases); they are separate, older downloads.

## Install or update from Switch, Windows or Mac

The installers download the latest packs from this repository. Select your pack and follow the app's installation steps.

| Installer | Download and use |
| --- | --- |
| **Switch — HOME menu** | [Nexus HATS Installer 1.0.1 NSP](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-n3/Nexus-HATS-Installer-1.0.1.nsp). Install it with your usual NSP installer. |
| **Switch — homebrew menu** | [Nexus HATS Installer 1.0.1 ZIP](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-n3/Nexus-HATS-Installer-1.0.1.zip). Extract onto the SD card and keep the support files together. |
| **Windows** | [Nexus HATS Desktop 1.0.1](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-n3/Nexus-HATS-Desktop.x64.exe). Run the standalone 64-bit EXE; no separate .NET installation is needed. |
| **Mac** | [Nexus HATS Desktop 1.0.1 DMG](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-n3/Nexus-HATS-Desktop-Universal.dmg). Supports Apple Silicon and Intel Macs on macOS 14 or later. Drag the app to Applications. |

**Update the installer before upgrading your pack.** Installer 1.0.1 preserves the USB mappings in `atmosphere/usb_content`, HOME badge data in `atmosphere/usb_badges`, and related repair/recovery files. It also prevents a downloaded pack from replacing these with another card's library data. HOC and supported system modules remain updateable.

Windows and Mac use the same [protection file](hats-exclusions.json); the Switch installer includes matching USB-library protections. These protections preserve existing data and do not recreate files that were already deleted.

The Mac app is not notarised. On first launch, macOS may require approval in **System Settings > Privacy & Security**.

## What's new

- **Current firmware base:** Atmosphere 1.12.2 with Switch 23.5.0 support, and official Hekate 6.5.5 / Nyx 1.9.5.
- **System-module compatibility:** avoids unnecessary USB checks during the startup of other modules, including the path involved in the SaltyNX boot investigation.
- **Cheat error handling:** several failed or malformed cheat operations can now stop cleanly instead of crashing the cheat service.
- **USB improvements retained:** sleep/wake recovery, write-performance changes, larger-library database handling, and SD/internal installation fixes while USB is connected.
- **Manager 0.2.16:** clearer navigation and storage labels, deletion fixes, and **Y — Delete all** in Cleanup with review and confirmation. Saved progress is kept.
- **Network and PC transfer:** saved SMB/NFS connections, queued network installs and FTP streaming to the chosen SD or USB destination, with live progress information.

See the [release notes](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/tag/v1.12.2-n3) for the full changes. Builds, automated checks and package verification passed. The latest compatibility, cheat and Manager deletion changes still need wider console testing.

## Included versions

| Component | Current pack |
| --- | --- |
| Nexus Atmosphere | **1.12.2 N3**, targeting Switch firmware **23.5.0** |
| Hekate / Nyx | **6.5.5 / 1.9.5**, official appearance |
| Nexus Manager | **0.2.16 R1**, NRO and native NSP |
| Nexus-compatible HOC | **2.6.0**, HOC pack only |
| Nexus USB Content overlay | **1.1.0**, with notification support |
| sys-patch | **1.6.3.0** |
| HATS installers | **1.0.1** for Switch, Windows and Mac |

## Getting started

You need a compatible modified Switch, a microSD card and a supported USB drive with a suitable connection and adequate power. Keep the drive connected while installing or playing its games. The pack does not install a Switch system firmware update or create an emuMMC for you.

1. Use an installer above, or shut down the Switch and extract **one** pack to the microSD root, replacing matching files. Preserve your Nintendo and emuMMC folders, USB mappings, saves, mods and cheats.
2. Boot through **Hekate > Launch** and choose your normal CFW entry. Use the included `payload.bin` for RCM injection. The emuMMC entry requires an existing emuMMC setup.
3. Open Nexus Manager from the homebrew menu. For its HOME-menu version, install **`install/Nexus-Manager-0.2.16.nsp`** from the pack. Copying the pack updates the NRO; it does not automatically reinstall the HOME-menu NSP.

When switching from an older HOC pack to No-HOC, disable the old HOC module's `atmosphere/contents/00FF0000636C6BFF/flags/boot2.flag`. If an old custom background remains, rename or remove `bootloader/res/background.bmp`. Extracting a new ZIP does not remove leftover modules or theme files.

The release packs do not include games, personal console keys, saves, backups or another user's USB mappings. GitHub's automatic **Source code** archives contain repository documentation, not the Switch pack.

## Other downloads

- [Nexus Manager 0.2.16 — NSP and NRO](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-n3/Nexus-Manager-0.2.16-R1.zip) for updating the app separately.
- [Nexus USB Formatter 1.6.1 for Windows](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v2026.11.04-sl7/Nexus-USB-Formatter-1.6.1-Windows.zip), supplied as a test build. Formatting erases the selected drive.
- [SHA-256 checksums](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-n3/SHA256SUMS.txt) for the current release downloads.

## Source and contributions

Help with building, testing and improving Nexus is welcome. Bug reports, documentation, code contributions and ideas for making the apps easier to use are appreciated.

| Project | Repository |
| --- | --- |
| Nexus Atmosphere firmware | [Nexus-Atmosphere](https://github.com/TR4UNEXUS/Nexus-Atmosphere) |
| Nexus USB driver and integration | [Nexus-USB-Firmware](https://github.com/TR4UNEXUS/Nexus-USB-Firmware) |
| Switch HATS Installer | [Nexus-HATS-Installer](https://github.com/TR4UNEXUS/Nexus-HATS-Installer) |
| Windows and Mac HATS Installer | [Nexus-HATS-Desktop](https://github.com/TR4UNEXUS/Nexus-HATS-Desktop) |

[Nexus Manager releases](https://github.com/TechRepairs4U/Nexus-Manager/releases) are maintained separately. The [earlier public Manager source snapshot](https://github.com/TR4UNEXUS/Nexus-Manager-Source) is not the source for every current binary release.

For a problem report, include the pack version, Switch firmware, HOC or No-HOC, whether the game is on SD or USB, and the exact error. Share relevant logs after removing personal information.

## Credits

Maintained by **TR4UNEXUS / TechRepairs4U**. Thanks to the [Atmosphere team](https://github.com/Atmosphere-NX/Atmosphere), [CTCaer and Hekate contributors](https://github.com/CTCaer/hekate), and the authors of the included HOC, overlay, sys-patch and homebrew components.

Third-party authorship and licence notices are retained in the packs and installer projects.
