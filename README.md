# LotJ Mudlet Packages

Seven ready-to-install packages from **Quiggly-Wiggly** for Legends of the Jedi.
One place to download them; each package has its own source repository.

**[Download all seven (.zip)](https://github.com/Quiggly-Wiggly/lotj-mudlet-packages/releases/latest/download/LotJ-Mudlet-Packages.zip)** · [All releases](https://github.com/Quiggly-Wiggly/lotj-mudlet-packages/releases)

## Pick your packages

Click a package name to download its `.mpackage`, or its description to view
source code, full setup instructions, and issue tracking.

| Package download | Version | First command | Source and documentation |
| --- | --- | --- | --- |
| [Buildship](https://github.com/Quiggly-Wiggly/lotj-mudlet-packages/releases/latest/download/LotJ.Buildship.mpackage) | v2.8.0 | `autobuild help` | [Shipbuilding queues and estimates](https://github.com/Quiggly-Wiggly/lotj-buildship) |
| [Autoflight](https://github.com/Quiggly-Wiggly/lotj-mudlet-packages/releases/latest/download/LotJ.Autoflight.mpackage) | v3.0.5 | `autoflight` | [Flights and saved landing preferences](https://github.com/Quiggly-Wiggly/lotj-autoflight) |
| [Doorways / setdoorway](https://github.com/Quiggly-Wiggly/lotj-mudlet-packages/releases/latest/download/LotJ.Doorways.mpackage) | v1.3.2 | `doorway ui` | [Saved door commands and mapper integration](https://github.com/Quiggly-Wiggly/lotj-doorways) |
| [Vendor Manager](https://github.com/Quiggly-Wiggly/lotj-mudlet-packages/releases/latest/download/LotJ.Vendor.Manager.mpackage) | v1.2.0 | `vendormgr` | [Examine entries, stock vendors, and set prices](https://github.com/Quiggly-Wiggly/le-examine) |
| [Auto Armor](https://github.com/Quiggly-Wiggly/lotj-mudlet-packages/releases/latest/download/LotJ.Auto.Armor.mpackage) | v2.3.1 | `autoarmor` | [Armor and enhancement queues](https://github.com/Quiggly-Wiggly/lotj-auto-armor) |
| [Cargo Scanner](https://github.com/Quiggly-Wiggly/lotj-mudlet-packages/releases/latest/download/lotj-cargoscanner.mpackage) | v0.4.0 | `cargoscan` | [Compare routes from your own scanned prices](https://github.com/Quiggly-Wiggly/lotj-cargoscanner) |
| [Comlink Crafter](https://github.com/Quiggly-Wiggly/lotj-mudlet-packages/releases/latest/download/LotJ.Comlink.Crafter.mpackage) | v1.5.0 | `mclhelp` | [Batch crafting, tuning, and container packing](https://github.com/Quiggly-Wiggly/lotj-comlink-crafter) |

## Install

1. Download the ZIP and extract it, or download individual packages above.
2. In Mudlet, open **Package Manager → Install New Package** and select each
   `.mpackage` you want. The collection ZIP itself is not a Mudlet package.
3. Connect to LotJ and use the first command listed above.

Requires **Mudlet 4.20+**. Install only the helpers you want. Doorways uses GMCP
room information and supports the standard LotJ mapper without custom edits.
Cargo Scanner needs GMCP planet data or the loaded LotJ UI galaxy map.

When updating, stop any active automation and uninstall that package's previous
version first. Remove old **Autoflight 2.0**, **Autobuildship**, **AutoArmor**, or
duplicate `le` / `givevendor` aliases before installing their replacements.
Vendor Manager retains the package ID `le-examine`; disable the old standalone
Vendor Giving alias with `lua disableAlias("Vendor Giving")`. Auto Armor keeps
the package ID `AutoArmorEnhanced`. Comlink Crafter retains `LotJComlink` and its
profile-local settings; finish any craft before upgrading. Each source README
explains retained settings and any session-only queues. Buildship estimates require your own learned values.

## What is included

Compact colored controls, visible commands, and setup links that prefill input
for review. The collection includes no characters, saved ship names, room rules,
landing pads, market snapshots, or learned recipe values. Examples are fictional;
configure each helper using your own game data.

This repository contains the installable packages and this guide. Code, tests,
change history, and issue tracking remain in the linked source repositories.
Each binary is copied unchanged from its tagged source release and checked against
that release's SHA-256 digest. Release checksums are attached as `SHA256SUMS.txt`.

**Collection v1.2.0** is a versioned snapshot of the packages listed above.
All seven source repositories passed their automated checks at publication; live
UI/gameplay checks remain manual. Check the source releases for changes published
after this collection. New collection releases update the table and downloads.
