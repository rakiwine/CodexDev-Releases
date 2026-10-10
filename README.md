# CodexDev Releases

Public distribution repository for **CodexDev Windows installers and signed updater assets**.

The application source code and build history are maintained separately in the private `rakiwine/CodexDev` repository. This public repository contains no application source, signing private keys or development credentials.

## Release assets

Each approved Windows x64 release contains:

- `CodexDev_<version>_x64-setup.exe` — Windows NSIS installer
- `CodexDev_<version>_x64-setup.exe.sig` — Tauri updater signature
- `latest.json` — signed-update feed metadata pointing to the versioned installer
- `manifest.json` — exact source commit, asset size and SHA-256 audit information

All assets are uploaded to a draft first, checked against the source build, and published only by a separate approval workflow. The updater signature and Windows Authenticode signature serve distinct verification purposes.

## Current status

**No production release has been published.** The application is in development, and the release pipeline must satisfy its license, security, signing, and Windows installation acceptance criteria before publication.

When a release is approved, it will appear in the [Releases](https://github.com/rakiwine/CodexDev-Releases/releases) section. Do not treat the existence of this repository as evidence that an installer has been validated.
