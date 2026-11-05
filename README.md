# AnoPOS releases

Desktop installers and packages for AnoPOS, and the signed update manifests the app reads to update itself.

- **Download:** pick the file for your system from the [latest release](https://github.com/AnoRebel/anopos-releases/releases/latest).
- **In-app updates:** AnoPOS reads `update-manifest.json` from the latest release. Every artifact in it carries an Ed25519 signature that the app checks against the key built into it before installing anything.
- **Verify a download by hand:** each file has a `.sigstore.json` bundle (`cosign verify-blob`) and is listed in `SHA256SUMS`.
