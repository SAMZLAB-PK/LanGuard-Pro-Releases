# Security Policy

LanGuard Pro controls router-management functions and may handle sensitive local-network credentials. Please treat security reports carefully.

## Supported release

Security fixes are prioritized for the latest public LanGuard Pro release listed in this repository.

## Reporting a security issue

Please **do not open a public GitHub issue** for vulnerabilities that expose credentials, permit unauthorized router control, bypass authentication, leak private network data, or otherwise create a meaningful security risk.

Instead, contact SAMZ Labs privately through the maintainer contact details available on the SAMZLAB-PK GitHub profile:

https://github.com/SAMZLAB-PK

When reporting privately, include:

- affected LanGuard Pro version
- Android version/device
- router model and firmware
- reproduction steps
- expected vs actual behavior
- logs with secrets removed

## Never send

Do not send real router passwords, private SSH keys, Play signing keys, API tokens, recovery codes, or other production secrets unless a secure channel has explicitly been agreed.

## Security model notes

LanGuard Pro uses Android Keystore-backed storage for remembered router credentials and pins/records SSH host identity so unexpected key changes can be surfaced instead of silently trusted.
