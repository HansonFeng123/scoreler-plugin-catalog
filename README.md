# Scoreler plugin catalog

The independent public plugin list for [Scoreler](https://github.com/HansonFeng123/Scoreler), a personal AI agent focused on studying.

Scoreler 1.4 and later can fetch `plugins.json` using **Toolbox > Plugins > Refresh plugin list**, without updating the whole application. Refreshing only updates the available list; installing or updating a plugin still requires review and confirmation. Scoreler keeps the last valid list locally and includes a bundled fallback for first use offline.

## Maintaining the list

Edit `plugins.json` on the `main` branch. Keep `schemaVersion: 1`, unique plugin IDs, GitHub author/repository identities, compatibility ranges, and ascending semantic release versions. Each release must use a published GitHub release tag `vX.Y.Z`, its matching ZIP download URL, and the ZIP's SHA-256. Retain historical releases. Never commit tokens, private configurations, user records, local paths or installers.

Scoreler validates the entire list before replacing its cache. Invalid JSON, unsupported metadata, unsafe download destinations, oversized responses, and network failures preserve the previous list. Packages continue to be checked against their catalog identity, release owner and SHA-256. Catalog inclusion and checksums are not a security audit.

## Current tools and credits

- [Graphing calculator](https://github.com/HansonFeng123/scoreler-graphing-calculator): based on Equation.io by Anthony Foster (MIT); see the plugin's full license and credits.
- [Offline Chinese-English translator](https://github.com/HansonFeng123/scoreler-offline-translator): credits and licenses for OPUS-MT, Transformers.js and ONNX Runtime are provided by the plugin.

## 中文

这是独立于 Scoreler 主程序的公开插件目录。Scoreler 1.4 起可在「百宝箱 → 插件 → 刷新插件列表」获取更新，无需更新整个应用。刷新只更新可用列表，不会自动安装或升级插件；离线时保留上次通过校验的目录，并提供内置列表作为备用。
