# LanGuard Pro Changelog

This file tracks public-facing LanGuard Pro release changes.

## 2.9.4 — versionCode 20905

### Reliability

- Fixed an SSH host-key repository bug that could surface as `NullPointerException: Attempt to get length of null array` during `SESSION_CONNECT`.
- Added guided SSH trust recovery for genuine host-key/trust failures, with a **Reset SSH Trust & Retry** path.
- Preserved normal authentication/network errors without incorrectly suggesting an SSH trust reset.
- Strengthened Companion and LuCI embedded-payload synchronization checks.

### Security

- Router passwords marked for saving use Android Keystore-backed encrypted storage instead of plain WebView local storage.
- Passwords are not permanently retained when **Remember password** is disabled.
- SSH trust follows a pinned/TOFU model instead of unconditional host-key acceptance.
- Privileged app WebView navigation remains restricted to local app content; external HTTP/HTTPS pages are handed off outside the privileged WebView.

### Live traffic

- Foreground Android Home/Devices refresh cadence aligned to 2 seconds.
- Per-device traffic accounting expanded to IPv4 + IPv6.
- IPv6 neighbor discovery is included so IPv6-active devices are less likely to appear with zero live speed.
- Counter reset/rebuild handling avoids carrying stale or ghost speed values into a new sample.

### Speed test

- Router-native speed-test support remains preferred when available.
- Cloudflare fallback behavior was bounded to reduce unnecessary parallel traffic while retaining a useful fallback path.

### LuCI

- Added official Google Play and SAMZ Labs public links to the LuCI LanGuard Pro page.
- Kept Companion/LuCI state integration aligned with the canonical router data path.

### Android / build

- App version updated to `2.9.4` / `20905`.
- `compileSdk` / `targetSdk` remain API 36.
- Android Gradle Plugin updated to the API-36-compatible 8.10.x line with Gradle 8.11.1.
- Removed Java API usages incompatible with the app's minimum Android level where identified.
- GitHub Actions supports manual workflow dispatch and produces debug APK / release bundle artifacts when run in an Android-capable runner.

## 2.9.3 — versionCode 20904

- API 36 migration baseline.
- Companion/LuCI synchronization and router service hardening.
- Background router monitoring and notification refinements.
- Multi-router profile persistence and WebView navigation/back behavior improvements.
