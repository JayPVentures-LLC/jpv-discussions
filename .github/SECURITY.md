# Security Policy

## Supported Scope

This repository (`jpv-discussions`) is a public community hub for discussions and documentation. It does not contain production application code. However, security issues related to:

- Exposed secrets or credentials accidentally committed to this repository
- Malicious content in community files, issue templates, or workflow files
- Vulnerabilities in GitHub Actions workflows (supply-chain attacks, script injection)
- Compromised CODEOWNERS or permission escalation paths

should be reported responsibly.

For security issues in JayPVentures production systems, infrastructure, or other repositories, use the GitHub Private Security Advisory path described below.

---

## Reporting a Vulnerability

**Do not open a public GitHub Issue to report a security vulnerability.**

### Preferred: GitHub Private Security Advisory

Use GitHub's built-in private reporting feature:
1. Navigate to the **[Security tab](../../security/advisories/new)** of this repository.
2. Click **"Report a vulnerability"**.
3. Fill in the advisory form. Your report will be visible only to repository maintainers.

### What to include in your report

- A clear description of the vulnerability
- Steps to reproduce or proof-of-concept
- Affected file(s), workflow(s), or component(s)
- Potential impact and severity assessment (see CVSS guidance below)
- Any suggested remediation (optional)

---

## Severity Classification

We use the following tiers to triage and prioritize reports:

| Severity | CVSS Score | Examples | Target Response |
|----------|-----------|---------|-----------------|
| **Critical** | 9.0 – 10.0 | Secret exposure, workflow takeover | Acknowledge in 24h; patch within 72h |
| **High** | 7.0 – 8.9 | Privilege escalation, data exfiltration path | Acknowledge in 48h; patch within 7 days |
| **Medium** | 4.0 – 6.9 | Information disclosure, supply-chain risk | Acknowledge in 72h; patch within 14 days |
| **Low** | 0.1 – 3.9 | Best-practice deviations, minor config issues | Acknowledge in 7 days; patch within 30 days |

---

## Response Process

1. **Acknowledgment** — We will confirm receipt of your report within the timeframe above.
2. **Assessment** — We will validate the report and assign a severity tier.
3. **Remediation** — A fix will be developed and tested.
4. **Disclosure** — After a fix is live, we will publish a security advisory crediting the reporter (unless anonymity is requested).
5. **Post-mortem** — For Critical/High findings, we will document lessons learned and preventive measures.

---

## Safe Harbor

JayPVentures will not pursue legal action against security researchers who:

- Discover and report vulnerabilities in good faith following this policy
- Avoid accessing, modifying, or deleting data that does not belong to them
- Limit testing to their own accounts and do not affect other users
- Do not disrupt services or share findings publicly before a fix is available

---

## Out of Scope

The following are not considered vulnerabilities for this repository:

- Missing security headers on GitHub.com itself (report to GitHub)
- Publicly known issues already tracked in open issues
- Theoretical vulnerabilities with no practical exploit path
- Issues requiring physical access to maintainer devices

---

## Acknowledgments

We appreciate the security research community's efforts to keep our systems and community safe. Confirmed vulnerability reporters may be acknowledged in the repository's security advisories with their consent.

