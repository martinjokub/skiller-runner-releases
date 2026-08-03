# Skiller Runner Manager releases

This public repository contains signed Windows installers and runner payloads for **Skiller Runner Manager**. Application and runner source code remain in private repositories.

Download the latest installer from [Releases](https://github.com/martinjokub/skiller-runner-releases/releases/latest).

Each release includes:

- an Authenticode-signed Windows NSIS installer;
- a runner payload ZIP used for independent per-profile updates;
- `runner-manifest.json` plus an Ed25519 signature;
- SHA-256 checksums.

The private release workflow refuses to publish when the Windows code-signing certificate, manifest signing key, or publishing token is missing. Skiller Runner Manager verifies the signed manifest and payload checksum before installing a runner version.