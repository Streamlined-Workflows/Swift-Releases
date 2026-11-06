# S.W.I.F.T. Releases

Installers for the S.W.I.F.T. desktop applications. This repository holds **no source code**: only finished,
checked installers and their checksums, published as GitHub Releases, plus the list the SWIFT Launcher reads to
install and update apps.

| Application | What it is |
|---|---|
| **SWIFT Launcher** | The front door to every S.W.I.F.T. product. Install this first: it is the only way into the desktop apps |
| **SWIFT Folio** | A desktop app to read, write, convert and build documents (part of S.W.I.F.T. Developer Tools). Install it from the Launcher |

## Installing

1. Download the **SWIFT Launcher** installer for your computer from the latest Launcher release.
   - Windows: `SWIFT Launcher Setup <version>.exe`
   - Linux: `SWIFT Launcher-<version>.AppImage`
2. Open the Launcher, sign in, and install the apps you have from there.

The installers are not code-signed yet. On Windows, SmartScreen warns the first time: choose **More info**,
then **Run anyway**. Check the download against its SHA-256 in the release's `SHA256SUMS.txt` if you want to
be sure it is the file published here.

## How releases are laid out (planned)

- One GitHub Release per application and version, tagged `launcher-v<version>` or `folio-v<version>`.
- Each release has the installers for each platform and a `SHA256SUMS.txt`.
- `latest.json` (in this repository) lists the current version of each application, with each installer's
  download address and SHA-256. The Launcher reads it to install and update apps, and refuses a file whose
  SHA-256 does not match.

## Licence

The S.W.I.F.T. applications are proprietary: see [LICENSE](LICENSE). The open-source components they include
keep their own licences: see [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).

© 2026 Streamlined Workflows & Innovation for Training L.L.C. All rights reserved.
