# Asnan Go — Update Channel

This repository is the **public update channel** for the Asnan Go desktop app.

It contains only:
- **`version.json`** — the update manifest (latest version number + the download link).
- **Releases** — each release has the `AsnanGo.exe` installer attached.

The app checks `version.json` on launch; if a newer version is listed, it offers
to download and install it automatically.

No source code or clinic data lives here — that stays private.

## Publishing a new version
1. Build the app (`release.py` in the private source repo) — it bumps the
   version and refreshes `version.json` here automatically.
2. Create a GitHub Release tagged `vX.Y.Z` and attach `AsnanGo.exe`
   (and the `AsnanGo-Setup-X.Y.Z.exe` installer).

Every clinic PC then sees the update on its next launch.
