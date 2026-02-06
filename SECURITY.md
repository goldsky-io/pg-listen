# Security Policy

## Purpose

This document tracks security vulnerabilities (CVEs) identified in our dependencies and our assessment of their applicability to our business. When Dependabot identifies a vulnerability, the owning team evaluates whether it poses a real risk given our usage patterns. This provides an audit trail for security decisions and ensures we can justify our risk assessments to auditors and compliance frameworks (SOC2, etc.).

## Vulnerability Remediation SLAs

According to our Vulnerability Management Policy, we follow these remediation timelines:

| Priority | SLA     |
|----------|---------|
| Critical | 30 days |
| High     | 30 days |
| Medium   | 60 days |
| Low      | 90 days |

## Process for Dismissed Alerts

When a vulnerability is determined to not apply to our usage:

1. The owning team dismisses the Dependabot alert with a reason
2. A follow-up PR is created to document the decision in this file
3. The entry below includes: CVE number, affected package, reason for dismissal, and the decision maker

This ensures we have documentation if:
- The vulnerability context changes and it later applies to us
- External auditors need to understand our security posture
- We need to re-evaluate decisions as our business expands

## Dismissed Alerts

The following vulnerabilities have been assessed and dismissed as tolerable risk (development dependencies not shipped to production):

| CVE | Alert | Package | Severity | Reason | Dismissed By | Date |
|-----|-------|---------|----------|--------|--------------|------|
| [CVE-2023-45133](https://nvd.nist.gov/vuln/detail/CVE-2023-45133) | [#27](https://github.com/goldsky-io/pg-listen/security/dependabot/27) | `@babel/traverse` | Critical | Development dependency - not shipped to production | @shreedhan | 2026-02-06 |
| [CVE-2023-45311](https://nvd.nist.gov/vuln/detail/CVE-2023-45311) | [#26](https://github.com/goldsky-io/pg-listen/security/dependabot/26) | `fsevents` | Critical | Development dependency - not shipped to production | @shreedhan | 2026-02-06 |
| [CVE-2021-44906](https://nvd.nist.gov/vuln/detail/CVE-2021-44906) | [#22](https://github.com/goldsky-io/pg-listen/security/dependabot/22) | `minimist` | Critical | Development dependency - not shipped to production | @shreedhan | 2026-02-06 |
| [CVE-2021-44906](https://nvd.nist.gov/vuln/detail/CVE-2021-44906) | [#21](https://github.com/goldsky-io/pg-listen/security/dependabot/21) | `minimist` | Critical | Development dependency - not shipped to production | @shreedhan | 2026-02-06 |
| [CVE-2022-25860](https://nvd.nist.gov/vuln/detail/CVE-2022-25860) | [#20](https://github.com/goldsky-io/pg-listen/security/dependabot/20) | `simple-git` | Critical | Development dependency - not shipped to production | @shreedhan | 2026-02-06 |
| [CVE-2020-7707](https://nvd.nist.gov/vuln/detail/CVE-2020-7707) | [#5](https://github.com/goldsky-io/pg-listen/security/dependabot/5) | `property-expr` | Critical | Development dependency - not shipped to production | @shreedhan | 2026-02-06 |
