# GigaBrain — Install & Updates

Public signed-installer update feed for the **GigaBrain** desktop app.

## Install or update (Windows)

Run this in PowerShell. It downloads the current signed installer from this feed, verifies it, and installs or updates GigaBrain. Git and Node.js are not required.

```powershell
$script = Join-Path $env:TEMP "Install-GigaBrain-Customer.ps1"; Invoke-WebRequest -UseBasicParsing "https://github.com/SethSummersTV/GigaBrain-Updates/releases/download/stable/Install-GigaBrain-Customer.ps1" -OutFile $script; powershell -NoProfile -ExecutionPolicy Bypass -File $script
```

This always installs the **latest** release — there is no version number to edit.

## Automatic in-app updates

Once GigaBrain is installed it updates itself. Open **Settings → App updates** and click **Check for updates**; the app pulls the latest signed installer from this feed automatically.

## Direct download

The **`stable`** release always holds the current customer build (`latest.yml`, `GigaBrain-Setup-<version>.exe`, and its `.blockmap`):

- Latest release & installer: https://github.com/SethSummersTV/GigaBrain-Updates/releases/tag/stable

Current version: **1.2.6**
