# Security Policy

## Supported versions

| Version        | Supported |
| -------------- | --------- |
| `0.1.x`        | Yes       |
| Older / forked | No        |

Current development version: `0.1.0-SNAPSHOT` (`jfx-annotations` module).

## Reporting a vulnerability

**Do not report security issues through public GitHub issues.**

1. **GitHub Private vulnerability reporting** (preferred)  
   Repository → **Security** → **Report a vulnerability**

2. **Email**  
   [arun.jakkam@vstack.co.in](mailto:arun.jakkam@vstack.co.in)

Reports are handled by **VStack** maintainers.

### What to include

- Description and impact
- Steps to reproduce
- Affected version or commit
- Suggested fix (optional)

### Response expectations

| Stage              | Target        |
| ------------------ | ------------- |
| Acknowledgement    | Within 7 days |
| Initial assessment | Within 14 days |
| Fix or mitigation  | Severity-based |

## Scope

In scope:

- **jfx-annotations** — runtime annotations under `com.vstack.jfx.annotations`
- Annotation retention or metadata issues that could affect binding security

Out of scope:

- Issues in **jfx-core** or **jfx-databind** (report to those repositories)
- Compile-time annotation processors (not shipped in this module)

## Security updates

Fixes are announced in release notes or GitHub Security Advisories when published.
