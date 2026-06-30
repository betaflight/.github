# Security Policy

Betaflight is an open-source project maintained by volunteers. We take the
security of the firmware, the app and supporting services seriously, and
we appreciate the efforts of security researchers and users who report issues
responsibly.

This is the canonical security policy for **all Betaflight repositories**.
Individual repositories may link here rather than duplicating it.

## Reporting a vulnerability

**Please do not report security vulnerabilities through public GitHub issues,
pull requests, Discord, or any other public channel.** Public disclosure before
a fix is available puts users at risk.

Instead, use one of the private channels below.

### 1. GitHub private vulnerability reporting (preferred, where enabled)

Many Betaflight repositories have GitHub's private vulnerability reporting
enabled. Where it is available:

1. Open the affected repository on GitHub.
2. Go to the **Security** tab → **Advisories** → **Report a vulnerability**.
   If you do not see a **Report a vulnerability** button, it is not enabled for
   that repository — use email instead.
3. Fill in the form with as much detail as you can (see below).

This keeps the report private to the maintainers and lets us collaborate with
you on a fix and a coordinated advisory.

### 2. Email

If private reporting is not enabled on the repository, you cannot use GitHub, or
your report concerns infrastructure rather than a specific repository, email:

**security@betaflight.com**

Email always works as a fallback, regardless of which repository is affected.

If you wish to encrypt your report, ask us for a current PGP key in an initial
(unencrypted) message containing no sensitive details.

## What to include

A good report helps us triage quickly. Where possible, please include:

- The affected component and version (firmware target and version, app version,
  commit hash, or the service/URL).
- A description of the issue and its security impact.
- Step-by-step reproduction instructions, a proof of concept, or affected code.
- Any logs, configuration, or hardware specifics needed to reproduce it.
- Your assessment of severity and any suggested remediation.

## Scope

This policy covers the projects maintained under the Betaflight organisation,
including but not limited to:

- **Firmware** — the flight controller firmware and its bootloader/option-byte
  handling.
- **The app** — the desktop, web, and mobile configurator applications.
- **Blackbox tooling and related utilities.**
- **Project infrastructure** — the website, build server, and release/update
  services.

### Out of scope

The following are generally **not** treated as Betaflight vulnerabilities.
Report them upstream where applicable:

- Vulnerabilities in third-party dependencies or vendor-supplied libraries
  (e.g. STM32/Pico HAL, mbedTLS) — report to the upstream project. If a
  Betaflight default exposes such an issue, we still want to hear about it.
- Issues requiring physical access or an already-compromised host, beyond the
  normal threat model of a USB-connected flight controller.
- Social engineering, spam, or volumetric denial-of-service against project
  infrastructure.
- Missing security hardening that has no demonstrated, exploitable impact.

If you are unsure whether something is in scope, report it anyway and let us
decide.

## Our commitment (coordinated disclosure)

As a volunteer project, we cannot guarantee fixed response times, but we aim to:

- **Acknowledge** your report within **5 business days**.
- Provide an **initial assessment** (including whether we consider it in scope)
  within **10 business days**.
- Keep you informed of progress while we work on a fix.
- Coordinate the timing of public disclosure with you. We aim to disclose within
  **90 days** of the initial report, or sooner once a fix is released. We will
  ask you not to disclose publicly before then.

We will publish a GitHub Security Advisory for confirmed vulnerabilities once a
fix or mitigation is available.

## Recognition

With your permission, we are happy to credit you in the security advisory and
release notes for responsibly disclosed vulnerabilities. Let us know how you
would like to be named, or if you prefer to remain anonymous.

Betaflight does not currently operate a paid bug bounty programme.

## Safe harbour

We consider security research and vulnerability disclosure conducted in good
faith and in accordance with this policy to be authorised. We will not pursue or
support legal action against researchers who:

- Make a good-faith effort to comply with this policy,
- Avoid privacy violations, data destruction, and service degradation, and
- Give us a reasonable opportunity to remediate before any public disclosure.

If in doubt about whether an action is acceptable, contact us first at
security@betaflight.com.
