# Security Policy

This document describes how to report security issues for projects in
the JavaScriptSolidServer organisation. Individual repositories may
publish their own `SECURITY.md` with project-specific contact paths or
scope; when they do, that overrides this one.

## Reporting a vulnerability

Please report security vulnerabilities **privately**, not via public
GitHub issues.

**Preferred contact:** open a [private security advisory][advisory] on
the affected repository. GitHub's Security Advisories let you discuss
the issue with maintainers in a private channel and coordinate a fix.

**Alternative:** email `melvincarvalho@gmail.com` with subject prefix
`[JSS SECURITY]` and a description of the issue. PGP-encrypted email is
welcome; key fingerprint available on request.

[advisory]: https://docs.github.com/en/code-security/security-advisories/working-with-repository-security-advisories/creating-a-repository-security-advisory

## What to include

- Affected repository and version (commit SHA or release tag)
- Description of the vulnerability and the threat model it enables
- Steps to reproduce (proof of concept where applicable)
- Suggested mitigation, if you have one
- Whether you intend to disclose publicly, and on what timeline

## Response expectations

- **Acknowledgement:** within 7 days of receipt
- **Initial assessment:** within 14 days
- **Coordinated disclosure window:** typically 90 days from initial
  report, longer if the issue requires substantial protocol or
  infrastructure changes. Shorter windows are negotiable for low-
  complexity issues.

We may publish an advisory crediting the reporter, with their consent.

## Scope

In scope for security disclosure:

- **Authentication and authorisation** — Solid-OIDC, NIP-98, WAC, JWT
  verification, DID resolution, profile-side verification methods
- **Server-side request forgery (SSRF)** — request paths that take
  user-controlled URLs or follow redirects
- **Data integrity / WAC bypass** — paths that allow reading or
  writing resources without correct ACL evaluation
- **Cryptographic correctness** — Schnorr signature verification, CID
  v1 multikey handling, hash usage
- **Supply chain** — dependency confusion, malicious package
  publication, account compromise vectors
- **Denial of service** — server-side resource exhaustion via crafted
  requests, oversized payloads, etc.

Out of scope (please do not file as security):

- Issues in third-party dependencies — file with the upstream project
  unless the issue is specific to how a JSS repository uses the
  dependency
- Self-XSS in the data browser via pasting attacker-controlled content
  into the user's own pod (the user is the attacker)
- Missing security headers on static asset paths where the asset
  itself is non-sensitive
- Anything requiring physical access or root on the user's own machine

## AGPL-3.0 §5(a) compliance

License-compliance issues on downstream forks (missing modification
notice on deployed modified versions) are **not** security issues. See
the relevant repository's `CONTRIBUTING.md` *"Forks and downstream
distribution"* section for the standard path, or open an issue against
the upstream repository for compliance discussion.

## Acknowledgements

Researchers who report security issues responsibly will be credited in
the relevant advisory unless they prefer to remain anonymous. We
appreciate the work it takes to find and report these issues
constructively.
