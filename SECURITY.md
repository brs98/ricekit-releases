# Security Policy

## Reporting a Vulnerability

Email **security@ricekit.app** with details. We aim to acknowledge within 48 hours and provide a fix or mitigation timeline within 7 days.

Please do **not** open public GitHub issues for security vulnerabilities.

## Scope

**In scope:**
- The RiceKit desktop app, CLI, and daemon binaries distributed from this repository
- The auto-update manifest and signature verification flow
- License activation and validation against LemonSqueezy

**Out of scope:**
- Issues that require physical access to an unlocked Mac
- Issues in third-party themes, templates, or integrations from `ricekit-community`
- Denial-of-service issues that require sending arbitrary network requests as the user
- Reverse engineering of the trial timer (this is a known limitation of any locally-enforced trial)

## Disclosure

We follow coordinated disclosure. After a fix ships, we will publish an advisory and credit the reporter (if they wish to be credited).
