# LanGuard Pro Support

Use this repository for **public release support**, reproducible bugs, installation problems, and compatibility reports.

## Before opening an issue

Please include:

- LanGuard Pro app version and version code.
- Android version and device model.
- Router model.
- OpenWrt/ImmortalWrt version.
- Whether the issue affects Android, LuCI, Companion, or more than one component.
- Clear reproduction steps.
- Relevant error text or screenshots with credentials removed.

For live-speed issues, also mention whether the affected device is Wi-Fi, Ethernet, Tailscale, IPv4, IPv6, or dual-stack if known.

For SSH installer issues, include the visible error text but **never include the router password, private keys, or authentication tokens**.

## Common SSH recovery case

If router firmware was reinstalled, SSH keys changed, or the router was replaced while keeping the same IP, LanGuard Pro may detect that the saved SSH identity no longer matches. Use the app's **Reset SSH Trust** recovery only when the app identifies a host-key/trust problem.

Do not use SSH trust reset as a workaround for a wrong password or an unreachable router.

## Distribution

Google Play is the recommended installation and update channel:

https://play.google.com/store/apps/details?id=com.samz.languardpro

Official standalone binaries, when published, will be attached to this repository's GitHub Releases.

## Private information

Do not post any of the following in public issues:

- Router/admin passwords
- SSH private keys
- API tokens
- Play signing/upload keys
- Private configuration backups
- Personally identifying network data that you do not want public

For sensitive security issues, follow [SECURITY.md](SECURITY.md).
