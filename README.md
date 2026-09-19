# Fortem releases

Public binary releases for [Fortem](https://fortem.dev), a local Kubernetes
environment inspector for macOS, Linux, and Windows.

Fortem runs on your machine, opens an embedded web UI on loopback, and connects
through an existing kubeconfig. It does not require a Fortem Helm chart or
in-cluster agent, and it starts read-only by default.

## Install

The canonical, reviewable instructions live at
[fortem.dev/install](https://fortem.dev/install). Release archives and
`checksums.txt` are attached on the [Releases](../../releases) page.

```sh
curl -fsSL https://fortem.dev/install.sh | sh
```

```powershell
irm https://fortem.dev/install.ps1 | iex
```

```sh
brew install cybrixcc/tap/fortem
```

The installer scripts verify the downloaded archive against the published
SHA-256 checksum. A checksum proves archive integrity; it is not code signing
or notarization. Current release security boundaries are documented at
[fortem.dev/security](https://fortem.dev/security).

This repository contains distribution artifacts only, not the Fortem source.
Use of the binaries is subject to the [Fortem terms](https://fortem.dev/terms).
