# SpaceBox

Official release builds for **SpaceBox** (SpaceBox Full), a private, end-to-end-encrypted vault for your files.

- Files are encrypted **on your device** with post-quantum cryptography (ML-KEM-768 key encapsulation + AES-256-GCM) before they are uploaded. The server only ever stores ciphertext, and your private key never leaves your device.
- Share files with contacts you add by QR code or invite code, transfer a file to a new owner, and take access back at any time.
- **Approvals**: require people you trust to agree before a file is shared or transferred. **Deadman's switch**: if you stop checking in, a file passes to the person you name.
- No email or phone number needed, no ads, no tracking.
- Works with [SpaceBox Lite](https://github.com/project-i46/spacebox-releases): receive files from Lite senders you approve, and send files to Lite boxes.

> **Note:** This repository hosts release binaries and documentation only. The application source code is not public.

## Download

Grab the latest version from the [**Releases**](../../releases/latest) page.

| Platform | File | Notes |
|----------|------|-------|
| Android | [Google Play](https://play.google.com/store/apps/details?id=com.spacebox.spaceboxFull)  | v1.0.12 |
| iOS | App Store for iPhone and iPad | coming soon |
| macOS | App Store for Mac | coming soon |
| Windows | `*.msix` | x64, code-signed |
| Linux | `*.run` | x64, self-contained installer |

## Installation

### Windows

Double-click the MSIX package and click **Install**. The package is code-signed (Azure Trusted Signing), so Windows App Installer accepts it directly. Requires Windows 10 (build 17763) or later, x64.

### Linux

Download the `.run` file, make it executable, and run it. It launches the installer:

```bash
chmod +x SpaceBoxFull-*-linux-x64.run
./SpaceBoxFull-*-linux-x64.run
```

## Updates

The app tells you when a new version is available here and links to its download. Installing it is the same as above.

## Verifying your download

Each release includes a `SHA256SUMS` file. After downloading, verify with:

```bash
sha256sum -c SHA256SUMS --ignore-missing
```

The Windows binary is additionally covered by its code signature (Azure Trusted Signing).

## Reporting problems

Found a bug or an installation issue? [Open an issue](../../issues) in this repository, or report it from inside the app. Please include your platform, app version, and what you were doing when the problem occurred, but **never attach your recovery file, its passphrase, private keys, contact or pairing codes, or session tokens**.

## Legal

SpaceBox is proprietary software, © i46. The binaries are provided as-is for end-user installation; redistribution of modified packages is not permitted.

[Terms of Use](https://www.i46.space/terms.html) · [Privacy Policy](https://www.i46.space/privacy.html)
