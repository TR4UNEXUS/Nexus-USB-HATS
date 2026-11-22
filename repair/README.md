# Nexus repair guidance

This catalogue helps Nexus Manager explain USB library problems and point users
to the right repair tool. It is intended for Manager **0.2.28 or newer**; use a
compatible Nexus firmware build for USB and console-backup support.

Open **Installed games > Repair USB games** for a preview. Manager checks the
local game, updates and DLC before changing missing library links. You can also
check the console map backup or scan for games missing from HOME.

Choose **Update repair guidance** to check for a newer catalogue. A bundled copy
and verified saved copies let the repair tools work without an internet connection.

The first catalogue covers missing library links, changed metadata, incomplete
files, missing registration, missing tickets and missing maps. It includes two
exact metadata variants from investigated reports. These are guidance entries,
not exceptions to file verification and not a guarantee that every title works.

- `catalog.nxrc` is the signed file read by Manager.
- `catalog.json` is its readable authoring data.
- `public-key.pem` is the public verification key.

There are no games, tickets, certificates, console keys or private server details
in this catalogue. It cannot run scripts, download game content or turn off
Manager's verification and rollback checks. The private signing key is not
published. Any changed catalogue must have a new revision and a valid signature.

Please [report problems](https://github.com/TR4UNEXUS/Nexus-USB-HATS/issues) with
the Manager/firmware versions and a diagnostic report. Help with reproducing
problems, checking repairs and improving the guidance is welcome.
