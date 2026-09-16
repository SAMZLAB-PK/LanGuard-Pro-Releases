# LanGuard Pro

**Official public release hub for LanGuard Pro by SAMZ Labs.**

LanGuard Pro is an Android + OpenWrt/ImmortalWrt network-management companion for monitoring connected devices, viewing live network activity, applying device controls, managing router services, and keeping LanGuard router components in sync.

> The main LanGuard Pro development repository is private. This public repository is intentionally limited to release information, public documentation, support links, changelogs, and official distribution references.

## Get LanGuard Pro

### Google Play

**Recommended installation method:**

https://play.google.com/store/apps/details?id=com.samz.languardpro

Package ID: `com.samz.languardpro`

### GitHub Releases

When a standalone APK is published by SAMZ Labs, it will appear in this repository's **Releases** section. Prefer Google Play for normal installations and updates.

## Current release

**LanGuard Pro 2.9.4**  
Version code: `20905`  
Target: Android 16 / API 36

Highlights:

- Safer SSH host-key handling with guided **Reset SSH Trust & Retry** recovery.
- Hardened router credentials using Android Keystore-backed encrypted storage.
- Improved per-device live-speed tracking with IPv4 + IPv6 accounting.
- 2-second foreground refresh cadence for Android Home/Devices and LuCI live views.
- Improved speed-test fallback behavior and reduced unnecessary parallel load.
- Updated LuCI LanGuard Pro page with official Google Play and SAMZ Labs links.
- Companion/LuCI payload synchronization and release-hardening checks.

See [CHANGELOG.md](CHANGELOG.md) for details.

## Router compatibility

LanGuard Pro is designed for supported OpenWrt/ImmortalWrt installations using the LanGuard Companion and LuCI LanGuard Pro components. Router compatibility depends on firmware, available packages, firewall/nftables support, and device architecture.

Before installing or repairing router components, make sure SSH access to the router is enabled and that you know the router's administrator credentials.

## Privacy

Privacy policy and public privacy documentation:

https://github.com/SAMZLAB-PK/LanGuard-Pro-Privacy

## Support

For installation problems, router compatibility questions, or reproducible bugs, see [SUPPORT.md](SUPPORT.md) and open an issue in this repository when appropriate.

Please do **not** post router passwords, SSH private keys, public IP addresses you consider sensitive, API tokens, Play signing keys, or other credentials in public issues.

## Security

Security-related guidance and private-reporting recommendations are in [SECURITY.md](SECURITY.md).

## Links

- SAMZ Labs: https://github.com/SAMZLAB-PK
- Google Play: https://play.google.com/store/apps/details?id=com.samz.languardpro
- Privacy: https://github.com/SAMZLAB-PK/LanGuard-Pro-Privacy

---

© 2026 SAMZ Labs. LanGuard Pro name, app branding, and release materials are maintained by SAMZ Labs.
