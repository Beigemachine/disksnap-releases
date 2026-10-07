# DiskSnap downloads

DiskSnap is a free Windows utility from [Beige Machine](https://beigemachine.com) for USB drives and SD cards. It has four tools: Backup, Restore, Clone and Make Bootable.

This repository holds the official installer downloads and their checksums. It does not contain DiskSnap's source code, which is not published.

## Download

Get the current installer from the [DiskSnap page on beigemachine.com](https://beigemachine.com/software/disksnap/) or from the [Releases page](../../releases/latest) of this repository.

| Version | File | Size | SHA-256 |
|---|---|---|---|
| 1.0.0 | `DiskSnap-1.0.0-setup.exe` | 37,689,920 bytes (35.9 MiB) | `F9A541FE94E835C4F9FE3F439D48BA981294B5E34AB8B13123FC03D8BDE85381` |

## Before you install

- DiskSnap is for 64-bit (x64) Windows PCs running a currently supported Windows 11 edition. It is not an ARM-native or 32-bit build.
- The installer includes the Microsoft .NET 10.0.12 runtime, so no separate runtime download is needed.
- The installer is unsigned. Windows may show an unknown-publisher warning or block it. Do not turn off Smart App Control, antivirus or other security protections to install DiskSnap.
- Restore, Clone and Make Bootable overwrite the destination drive. Check the source and destination carefully and keep another copy of important data.

Full instructions: [Install DiskSnap](https://beigemachine.com/docs/disksnap/install/) and the [user manual](https://beigemachine.com/docs/disksnap/user-manual/).

## Check your download

In PowerShell, with the path to the file you downloaded:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath 'C:\path\to\DiskSnap-1.0.0-setup.exe'
```

The value must match the SHA-256 above. A checksum shows that your copy matches the published file. It is not a digital signature.

## Licence

DiskSnap is freeware: all four tools are free for personal and business use, and donations are optional. The terms are in [DiskSnap-licence.txt](DiskSnap-licence.txt). They are also shown during Setup and installed with DiskSnap, together with the notices for Microsoft .NET and the bundled fonts.

Please link to the Beige Machine download page instead of re-hosting the installer.

GitHub adds "Source code" archives to every release automatically. Those archives contain only the files in this repository, not DiskSnap's source code.

## Help

Email beigemachine@gmail.com with your DiskSnap version, Windows version and the exact error message. Do not send passwords or private files.
