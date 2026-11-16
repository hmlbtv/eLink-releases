# eLink releases (public downloads)

Installers and firmware files for eLink nameplates. Nothing secret is stored here: firmware is published **unsigned**; the eLink Manager signs it on your own computer with your own key.

| What | File |
|---|---|
| eLink Manager for Windows | `app/eLink-Manager-Setup-<version>.exe` |
| Pico firmware (unsigned source files) | `firmware/elink-firmware-v<N>.zip` |
| List of every release with sizes and SHA-256 | `releases.json` |

The eLink Manager reads `releases.json` and shows only releases that are newer than what you have.

To install the Manager by hand: open the `.exe` here, press the download button, run it. Windows may warn because the installer is not signed (More info, then Run anyway).
Check a download: `certutil -hashfile eLink-Manager-Setup-<version>.exe SHA256` and compare with `releases.json`.
