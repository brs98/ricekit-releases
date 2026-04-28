# RiceKit Releases

This repository distributes signed, notarized macOS binaries for [RiceKit](https://ricekit.app).

The RiceKit source code is closed and lives in a private repository. Only release artifacts are published here — DMG installers and the auto-update manifest.

## Install

Download the latest DMG from [Releases](https://github.com/brs98/ricekit-releases/releases/latest) or use the stable redirect once the marketing site is live:

```
https://download.ricekit.app/latest
```

After mounting the DMG, drag **RiceKit.app** into `/Applications` and launch it. You'll get a 7-day full-feature trial — no account or credit card required.

## Verify the signature

Every release is signed with a Developer ID certificate and notarized by Apple. To verify a downloaded DMG before opening:

```bash
spctl --assess --type install RiceKit-<version>.dmg
codesign --verify --verbose=4 /Applications/RiceKit.app
```

## Auto-updates

The desktop app updates itself via a manifest at:

```
https://update.ricekit.app/latest.json
```

Format follows the [Tauri updater spec](https://v2.tauri.app/plugin/updater/).

## Buy a license

After the trial ends, activate a license to keep using RiceKit. $34 one-time, no subscription, one license activates up to 2 Macs.

[Buy RiceKit →](https://buy.ricekit.app)

## Support

- **Bug reports:** [open an issue](https://github.com/brs98/ricekit-releases/issues/new/choose)
- **Themes, templates, integrations:** PRs welcome at [ricekit-community](https://github.com/brs98/ricekit-community)
- **Security disclosures:** see [SECURITY.md](./SECURITY.md)
- **Licensing & billing:** brandon@ricekit.app

## License

The binaries published here are © Brandon Southwick. All rights reserved. See [LICENSE.md](./LICENSE.md).

The themes, templates, and integrations bundled with RiceKit live in the public [ricekit-community](https://github.com/brs98/ricekit-community) repo and are governed by their own licenses.
