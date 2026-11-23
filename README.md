# Nexus USB HATS

Install and play games from external USB storage on a compatible modified Nintendo Switch.

**Nexus Atmosphere 1.12.2 RF2 · Switch firmware 23.5.0 support · Hekate 6.5.5 / Nyx 1.9.5 · Nexus Manager 0.2.30**

[Download the latest release](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/latest) · [What's changed](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/tag/v1.12.2-rf2) · [Report a problem](https://github.com/TR4UNEXUS/Nexus-USB-HATS/issues)

Keep a larger game library on an external HDD, SSD or USB flash drive. Your microSD card still holds the console setup and the information that connects your USB library to the system.

## Choose a pack

The two **Standard** packs use the official Hekate/Nyx appearance and original Atmosphere splash. **Nexus-themed HOC** adds the custom Nexus Hekate/Nyx menu, the original purple Nexus Atmosphere splash, and distinct EMU / SYS CFW Launch icons. All three include the same current Nexus USB firmware, Manager and USB Content overlay.

| Pack | Choose it if… |
| --- | --- |
| [**Standard No-HOC**](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-rf2/Nexus-1.12.2-RF2-Standard-No-HOC.zip) | You want Nexus USB support without HOC's clock controls. |
| [**Standard HOC**](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-rf2/Nexus-1.12.2-RF2-Standard-HOC.zip) | You also want the included Horizon OC 2.6.1 and its overlay. |
| [**Nexus-themed HOC**](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-rf2/Nexus-1.12.2-RF2-Nexus-Themed-HOC.zip) | You want Standard HOC with the custom Nexus Hekate/Nyx appearance, restored Nexus splash and EMU / SYS CFW Launch icons. |

This three-pack lineup is the default for future releases.

Choose **one** pack. All three include Nexus Manager as an NRO and installable NSP, the USB Content overlay with coloured notifications, sys-patch, Nintendo DNS rules, and ready-made Hekate Launch entries.

These are the three current pack choices. The older Full and themed packs remain in [previous releases](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases); they are separate, older downloads.

## Install or update from Switch, Windows or Mac

The installers download the latest packs from this repository. Select your pack and follow the app's installation steps.

| Installer | Download and use |
| --- | --- |
| **Switch — HOME menu** | [Nexus HATS Installer 1.0.3 NSP](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-rf2/Nexus-HATS-Installer-1.0.3.nsp). Install it with your usual NSP installer. |
| **Switch — homebrew menu** | [Nexus HATS Installer 1.0.3 ZIP](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-rf2/Nexus-HATS-Installer-1.0.3.zip). Extract onto the SD card and keep the support files together. |
| **Windows** | [Nexus HATS Desktop 1.0.1](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-rf2/Nexus-HATS-Desktop.x64.exe). Run the standalone 64-bit EXE; no separate .NET installation is needed. |
| **Mac** | [Nexus HATS Desktop 1.0.1 DMG](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-rf2/Nexus-HATS-Desktop-Universal.dmg). Supports Apple Silicon and Intel Macs on macOS 14 or later. Drag the app to Applications. |

**Update the installer before upgrading your pack.** Switch Installer 1.0.3 and Desktop Installer 1.0.1 preserve the USB mappings in `atmosphere/usb_content`, HOME badge data in `atmosphere/usb_badges`, and related repair/recovery files. They also prevent a downloaded pack from replacing these with another card's library data. HOC and supported system modules remain updateable.

Windows and Mac use the same [protection file](hats-exclusions.json); the Switch installer includes matching USB-library protections. These protections preserve existing data and do not recreate files that were already deleted.

The Mac app is not notarised. On first launch, macOS may require approval in **System Settings > Privacy & Security**.

## What's new

- **Homebrew launches restored:** RF2 fixes Album opening the normal gallery and hold-R launches missing the Homebrew Menu after the loader separation. Normal mod and button checks work through the separate loader again.
- **USB transfer reliability:** fixes a case where an already-completed transfer could be reported as a timeout after a missed notification.
- **Manager 0.2.30:** clearer firmware, storage and connection errors; more reliable moves when matching files are already present; and more useful failure reports.
- **Bulk deletion and relinking:** select several games to delete while keeping saved progress, or use Tickets + link existing files with a suitable original package when the complete game content is already on a drive.
- **Retained features:** USB map backups to console storage, repair guidance, language selection, USB Content 1.3.0 with safe eject and coloured notifications, and the existing sleep/wake, compressed game-data and cheat-service fixes.
- **Separate HOC and themed boot:** both HOC packs retain Horizon OC 2.6.1 separately from Nexus USB. The themed pack retains the compressed Nexus splash and EMU / SYS Launch icons.
- **Installers and Formatter:** the current Switch, Windows and Mac installers and USB Formatter remain available together in this release.

See the [release notes](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/tag/v1.12.2-rf2) for update instructions. Build and automated checks passed; RF2 and Manager 0.2.30 still need console testing. Please report bugs with logs or a Manager diagnostic report.

**Nextendo users:** after updating HATS, reopen Prelude, reapply Nextendo mode and follow its restart instructions. A pack update can replace the network settings it needs. The relevant DNS and mod-loading paths are retained, but Nextendo's own firmware restrictions still apply. See [Prelude's source and setup information](https://git.nextendo.network/NextendoNetwork/Prelude-Nextendo).

## Included versions

| Component | Current pack |
| --- | --- |
| Nexus Atmosphere | **1.12.2 RF2**, targeting Switch firmware **23.5.0** |
| Hekate / Nyx | **6.5.5 / 1.9.5**, official or custom Nexus appearance |
| Nexus Manager | **0.2.30**, NRO and native NSP |
| Horizon OC | **2.6.1**, separate from Nexus USB, both HOC packs |
| Nexus USB Content overlay | **1.3.0**, drive information and safe eject |
| sys-patch | **1.6.3.0** |
| HATS installers | **1.0.3** for Switch; **1.0.1** for Windows and Mac |

## Getting started

You need a compatible modified Switch, a microSD card and a supported USB drive with a suitable connection and adequate power. Keep the drive connected while installing or playing its games. The pack does not install a Switch system firmware update or create an emuMMC for you.

1. Use an installer above, or shut down the Switch and extract **one** pack to the microSD root, replacing matching files. Preserve your Nintendo and emuMMC folders, USB mappings, saves, mods and cheats.
2. Boot through **Hekate > Launch** and choose your normal CFW entry. Use the included `payload.bin` for RCM injection. The emuMMC entry requires an existing emuMMC setup.
3. Open Nexus Manager from the homebrew menu. For its HOME-menu version, install **`install/Nexus-Manager-0.2.30.nsp`** from the pack. Copying the pack updates the NRO; it does not automatically reinstall the HOME-menu NSP.

When switching from an older HOC pack to No-HOC, disable the old HOC module's `atmosphere/contents/00FF0000636C6BFF/flags/boot2.flag`. If an old custom background remains, rename or remove `bootloader/res/background.bmp`. Extracting a new ZIP does not remove leftover modules or theme files.

The release packs do not include games, personal console keys, saves, backups or another user's USB mappings. GitHub's automatic **Source code** archives contain repository documentation, not the Switch pack.

## Other downloads

- [Nexus Manager 0.2.30 — NSP and NRO](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-rf2/Nexus-Manager-0.2.30-R1.zip) for updating the app separately.
- [Nexus USB Formatter 1.6.1 for Windows](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-rf2/Nexus-USB-Formatter-1.6.1-Windows.zip). Formatting erases the selected drive.
- [SHA-256 checksums](https://github.com/TR4UNEXUS/Nexus-USB-HATS/releases/download/v1.12.2-rf2/SHA256SUMS.txt) for the current release downloads.

## Source and contributions

Help with building, testing and improving Nexus is welcome. Bug reports, documentation, code contributions and ideas for making the apps easier to use are appreciated.

| Project | Repository |
| --- | --- |
| Nexus Atmosphere firmware | [Nexus-Atmosphere](https://github.com/TR4UNEXUS/Nexus-Atmosphere) |
| Nexus USB driver and integration | [Nexus-USB-Firmware](https://github.com/TR4UNEXUS/Nexus-USB-Firmware) |
| Switch HATS Installer | [Nexus-HATS-Installer](https://github.com/TR4UNEXUS/Nexus-HATS-Installer) |
| Windows and Mac HATS Installer | [Nexus-HATS-Desktop](https://github.com/TR4UNEXUS/Nexus-HATS-Desktop) |

[Nexus Manager releases](https://github.com/TechRepairs4U/Nexus-Manager/releases) use a separate auto-update feed. Manager 0.2.30 is included in this HATS release and its standalone download above. The [Manager source repository](https://github.com/TR4UNEXUS/Nexus-Manager-Source) is maintained separately.

For a problem report, include the pack version, Switch firmware, HOC or No-HOC, whether the game is on SD or USB, and the exact error. Share relevant logs after removing personal information.

## Credits

Maintained by **TR4UNEXUS / TechRepairs4U**. Thanks to the [Atmosphere team](https://github.com/Atmosphere-NX/Atmosphere), [CTCaer and Hekate contributors](https://github.com/CTCaer/hekate), and the authors of the included HOC, overlay, sys-patch and homebrew components.

Third-party authorship and licence notices are retained in the packs and installer projects.

