# Skiller Runner binary releases

This public repository is the binary-distribution channel for two independently versioned products:

- **Skiller Runner** — native execution payloads tagged `runner-vX.Y.Z`.
- **Skiller Runners Manager for Windows** — installable tray application tagged `manager-windows-vX.Y.Z`.

Runner and Manager source code remain private in the canonical Skiller monorepo. This repository contains no editable application source and is not a second Runner repository.

## Download

Open [Releases](https://github.com/martinjokub/skiller-runner-releases/releases) and select the product-specific tag:

- For a new Windows installation, choose the newest `manager-windows-v...` release and download `Skiller-Runners-Manager-...-x64.exe`.
- Runner payloads under `runner-v...` are normally downloaded and verified automatically by the installed Manager.

Do not use a repository-wide “latest release” link: Runner and Manager releases share this repository but have separate version lines.

## Verification

Every product release includes an Ed25519-signed manifest, SHA-256 checksums, the approved INTERNET IDEAS LTD EULA, and reviewed third-party notices. Manager installers are additionally Authenticode-signed; Windows must report the expected publisher as **INTERNET IDEAS LTD**.

The public verification key is committed at [`runner-release-public-key.pem`](runner-release-public-key.pem). The installed Manager embeds the same trust root and rejects invalid signatures, product/tag mismatches, unsafe assets, or checksum/size mismatches.

## Ownership

Skiller Runner and Skiller Runners Manager are proprietary software of **INTERNET IDEAS LTD**. AI Masters Apps is a brand operated by INTERNET IDEAS LTD. The licence included with each release controls use and distribution of the binaries.

## Security

Do not report vulnerabilities in a public issue. Follow [`SECURITY.md`](SECURITY.md) and use GitHub private vulnerability reporting.
