# Fortem releases

Public binary releases for [Fortem](https://fortem.dev), a local Kubernetes
environment inspector for macOS, Linux, and Windows.

Fortem runs on your machine, opens an embedded web UI on loopback, and connects
through an existing kubeconfig. It does not require a Fortem Helm chart or
in-cluster agent, and it starts read-only by default.

## Install

Release archives, installer scripts, and `checksums.txt` are attached on the
[Releases](../../releases) page. The GitHub-hosted commands below work before
the new fortem.dev website is promoted to production.

```sh
curl -fsSL https://github.com/cybrixcc/fortem-releases/releases/latest/download/install.sh | sh
```

```powershell
irm https://github.com/cybrixcc/fortem-releases/releases/latest/download/install.ps1 | iex
```

```sh
brew install cybrixcc/tap/fortem
```

The installer scripts verify the downloaded archive against the published
SHA-256 checksum. A checksum proves archive integrity; it is not code signing
or notarization. Current release security boundaries are documented at
[fortem.dev/security](https://fortem.dev/security).

The shorter `fortem.dev/install.sh` and `install.ps1` URLs become canonical
when the Kubernetes website PR is promoted. Both copies are byte-for-byte the
same scripts for this release.

This repository contains distribution artifacts only, not the Fortem source.
The Fortem Local Binary License and third-party notices are included in every
archive. Use of the website and services is also subject to the
[Fortem terms](https://fortem.dev/terms).
