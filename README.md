# Windows Updates Downloader (WUD)

<img width="1210" height="965" alt="WUD v8.0" src="https://github.com/user-attachments/assets/f9f73702-b2c0-489f-b571-087a891a9c53" />

## Description
WUD is a utility to download updates and vendor binaries from update lists (.ul files). It includes download reliability improvements and UI options to control behaviour.

## History
This is a small program originally created by Jean-Sebastien Carle that I have decided to update and maintain that allows you to download and install all of the current Windows critical updates, Microsoft Programs and now in version 8.0 Graphics Card Drivers. All files are downloaded directly from Microsoft's new CDN servers. GPU Drivers# are downloaded from NVIDIA, AMD and Intel to your computer with a single mouse click.

**#Feature only available in WUD v8.0 or above.**

## Key user-visible changes
- Improved download reliability
- Conservative, browser-like request behaviour is used for better compatibility with CDN servers like Microsoft, AMD and Intel.
- An option to suppress per-file error popups is available; when enabled, WUD shows a single summary of the download failure.
- UI layout adjusted to prevent overlapping controls at common display scales.
- Theme support for both Dark and Light modes and detects what theme settings Windows 10 or 11 is set too, when launched this is on by default.
- Download optimizations for NVIDIA downloads, this is on by default with the option to turn off in the settings.

## Please note
This repository is closed-source. No source code will be shared.

## Support
If a download still fails, check `download.log` in the application's local data folder for troubleshooting entries and open a private issue with log excerpts
