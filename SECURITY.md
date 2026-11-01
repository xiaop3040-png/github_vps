# Security guidance

This repository demonstrates development environments and remote access. **Do not deploy its example credentials to an Internet-facing host.**

## Before use

- Replace all default passwords with unique, strong secrets; never commit real credentials.
- Prefer SSH public-key authentication; disable password-based root SSH access where possible.
- Use a private network such as Tailscale for SSH, RDP and administrative interfaces. Do not expose ports 22, 3389, 4200 or 8006 broadly.
- Apply operating-system and dependency updates and enable host firewalls.
- Restrict access to trusted identities, use MFA where supported, and rotate any exposed credentials.
- Review GitHub Actions permissions, third-party actions and repository secrets before running workflows.
- Do not store persistent secrets in logs, screenshots, README examples or artifacts.

## Reporting

If you discover a security issue, avoid posting credentials or exploit details in a public issue. Contact the repository maintainer through their GitHub profile to arrange private disclosure.
