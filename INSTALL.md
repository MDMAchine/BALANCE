# Installing BALANCE

No installer is needed. Download the zip for your platform from the [Releases page](../../releases/latest) and unzip it.

## Windows

1. Copy `Win/VST3/BALANCE.vst3` (the whole folder) into `C:\Program Files\Common Files\VST3`.
2. Copy `Win/CLAP/BALANCE.clap` into `C:\Program Files\Common Files\CLAP`.
3. Rescan plugins in your DAW.
4. The standalone app, `Win/Standalone/BALANCE.exe`, runs directly.

The binaries are not code-signed, so SmartScreen may show "Windows protected your PC". Click "More info", then "Run anyway". It will not ask again for the same file.

## macOS

1. Copy `Mac/AU/BALANCE.component` into `~/Library/Audio/Plug-Ins/Components`.
2. Copy `Mac/VST3/BALANCE.vst3` into `~/Library/Audio/Plug-Ins/VST3`.
3. Copy `Mac/CLAP/BALANCE.clap` into `~/Library/Audio/Plug-Ins/CLAP`.
4. Quit and reopen your DAW. In Logic Pro, use Logic > Settings > Plug-in Manager > Reset & Rescan All.
5. The standalone app, `Mac/Standalone/BALANCE.app`, can go anywhere, for example Applications.

The Mac binaries are ad-hoc signed but not notarized. If macOS says the plugin is damaged or cannot be opened, allow it under System Settings > Privacy & Security, or clear the quarantine flag in Terminal, for example:

```
xattr -dr com.apple.quarantine ~/Library/Audio/Plug-Ins/Components/BALANCE.component
```

Run the same command for the VST3, CLAP and app paths you installed.

## Checking the download

Each zip has a `SHA256SUMS.txt` listing every file inside. The zip hashes themselves are listed in the release notes.
