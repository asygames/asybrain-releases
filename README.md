# AsyBrain Releases

Public downloads for the AsyBrain native Connector, desktop Agent and installer scripts. Releases are built and verified locally; GitHub Actions is not used.

## Downloads

| Product | Current download | Update channel |
| --- | --- | --- |
| Background Connector — Windows x64 / Linux x64 | [Connector 0.2.56](https://github.com/asygames/asybrain-releases/releases/tag/asybrain-connector-v0.2.56) | [Signed stable manifest](https://github.com/asygames/asybrain-releases/releases/download/asybrain-connector-stable/latest.json) |
| Installer scripts — PowerShell, CMD and Linux | [Installer 0.1.2](https://github.com/asygames/asybrain-releases/releases/tag/asybrain-installer-v0.1.2) | [Installer channel](https://github.com/asygames/asybrain-releases/releases/tag/asybrain-installer-stable) |
| Desktop Agent — historical desktop client | [Desktop releases](CATALOG.md#desktop-agent) | [Signed desktop manifest](https://github.com/asygames/asybrain-releases/releases/download/asybrain-agent-stable/latest.json) |
| AsyIndex Hub — retired | [Historical downloads](CATALOG.md#asyindex-hub-archive) | Archive only; no maintained automatic updates |
| Legacy Relay distribution | [Historical downloads](CATALOG.md#legacy-relay) | Current Relay updates are published by the website source repository |

Use the product links above: the generic GitHub “Latest” release may refer to the installer rather than the native Connector. Installer, npm package, Connector, desktop Agent and Relay version numbers are independent.

Quick install instructions and account approval: [asybrain.win](https://asybrain.win). Published files include their checksums; native stable manifests retain their existing signing identity.

## Source and archive

- Native Agent, Connector and installer source: [asygames/asybrain-relay-agent](https://github.com/asygames/asybrain-relay-agent).
- Website and current Relay source: [asygames/asybrain](https://github.com/asygames/asybrain).
- Retired Hub source: private `asygames/asyindex`; historical binaries remain available here.
- [Full release catalog](CATALOG.md) and [compatibility / retention policy](COMPATIBILITY.md).

This repository was renamed from `asygames/asyindex-releases`; its immutable GitHub repository ID is **1373532789**. The rename preserves its history, tags and release assets.
