# Windows Updates Downloader (WUD)

<img width="1210" height="1002" alt="WUD-v6 0 1204" src="https://github.com/user-attachments/assets/1569a7fe-e806-41a9-b1e9-2b5fc1ef8e7d" />

## Description
WUD is a utility to download updates and vendor binaries from update lists (.ul files). It includes download reliability improvements and UI options to control behavior.

## History
This is a small program originally created by Jean-Sebastien Carle that I have decided to update and maintain that allows you to download and now install all of the current Windows critical updates and programs. All updates and programs are downloaded directly from Microsoft's new CDN servers to your computer with a single mouse click.

## Key user-visible changes
- Improved download reliability
- Conservative, browser-like request behaviour is used for better compatibility with CDN edges.
- An option to suppress per-file error popups is available; when enabled, WUD shows a single summary at the end of a download run.
- UI layout adjusted to prevent overlapping controls at common display scales.

## Privacy note
This repository is closed-source. No source code will be shared.

## Usage
- Use the Options area to configure behavior.
- The application persists user options between runs.

## Support
If a download still fails, check `download.log` in the application's local data folder for troubleshooting entries and open a private issue with log excerpts
