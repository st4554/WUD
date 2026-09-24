# Windows Updates Downloader (WUD)

## Description
WUD is a utility to download updates and vendor binaries from update lists (.ul files). It includes download reliability improvements and UI options to control behavior.

## History
This is a small program originally created by Jean-Sebastien Carle that I have decided to update and maintain that allows you to download and now install all of the current Windows critical updates and programs. All updates and programs are downloaded directly from Microsoft's new CDN servers to your computer with a single mouse click.

## Key user-visible changes
- Improved download reliability
- Conservative, browser-like request behaviour is used for better compatibility with CDN edges.
- An option to suppress per-file error popups is available; when enabled, WUD shows a single summary at the end of a download run.
- UI layout adjusted to prevent overlapping controls at common display scales.

## Notable changes (2026-09-14)
This release contains several performance, reliability, and UX improvements to the download subsystem and settings UI.

- **New settings**
- `SuppressPerFileMessages` (Program): default `false`. When enabled, per-file MessageBox popups for failures are suppressed, and a single summary is shown at the end of the queue. Useful for automated or bulk downloads.

- **Download performance and reliability**
  - Increased default per-download buffer from 8 KB to 256 KB for improved throughput on modern networks and large files.
  - When a Microsoft CDN is detected, the manager increases the buffer to 1 MB for better single-connection throughput.

- **Logging and diagnostics**
  - The download manager writes diagnostic logs to `%LOCALAPPDATA%\Supremus Corporation\Windows Updates Downloader\download.log`.

- **Installer integration**
  - When `Download and Install` is used, downloaded files (`.msu`, `.exe`, `.cab`) are invoked with quiet/no-restart switches where applicable (`wusa.exe` for MSU, `dism.exe` for CAB).

- **System Requirements**
  - `Microsoft .NET Framework 4.8.1`.
  - Settings keys: `Program.SuppressPerFileMessages` are read/written in the Settings section of the application settings.

## Privacy note
This repository is closed-source. No source code will be shared.

## Usage
- Use the Options area to configure behavior.
- The application persists user options between runs.

## Support
If a download still fails, check `download.log` in the application's local data folder for troubleshooting entries and open a private issue with log excerpts
