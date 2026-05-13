# Contributing to JavaScriptSolidServer projects

This is the organization-wide default. Individual repositories may
publish their own `CONTRIBUTING.md` with project-specific Quick start
and Code style sections (e.g. the JSS server repo); when they do, that
overrides this one. The sections below apply universally.

## Workflow

Projects follow a strict **issue → branch → PR → merge → pull**
sequence. No direct commits to the default branch.

1. Open an issue describing the change (or pick an existing one)
2. Branch: `git checkout -b issue-<number>-short-slug`
3. Commit with a descriptive title + multi-paragraph body explaining
   the *why*
4. Open a PR linked to the issue
5. Address Copilot review iteratively until clean (the org leans
   heavily on automated review passes)
6. Squash-merge, delete branch, `git pull`

## AI-assistance disclosure

We welcome thoughtfully-prepared contributions, including those drafted
with AI assistance. To keep provenance clear:

- **Disclose AI assistance** in the PR description. Indicate one of:
  - hand-authored
  - AI-assisted with substantive human review
  - substantially AI-generated
- **Share prompts** for substantial AI-generated portions (in the PR
  description or a linked artifact) so reviewers can assess scope.
- **Authorship responsibility** — code review, follow-up, and licence
  obligations stay with the contributor regardless of AI involvement.
- **Per-contributor flexibility** — established contributors with a
  consistent disclosure history may agree streamlined arrangements
  with the maintainer.

This is consistent with [NLnet's generative-AI policy for funded
projects](https://nlnet.nl/foundation/policies/generativeAI/) and
general open-source provenance best practice.

A pull-request template (`.github/pull_request_template.md`) carries
the same checklist so every PR captures the disclosure inline.

## Forks and downstream distribution

Projects in this org are AGPL-3.0. Forks are welcome.

The licence terms set the boundary: **§5(a)** requires a prominent
modification notice on conveyed (deployed, published, or distributed)
modified versions, with a relevant date. Forks operating a public
deployment are encouraged to surface this notice on the deployment
itself — about page, footer, response headers, or equivalent — so
downstream users have visible provenance.

If you are forking and want to ensure §5(a) compliance, please open
an issue or ping the maintainer; happy to advise on how to apply the
notice cleanly.

## Licence and CLA

All projects in this org are licensed under AGPL-3.0 (see each
repository's `LICENSE`). Contributions are accepted under the same
licence by default.

A Contributor Licence Agreement is being drafted and will be required
for substantial contributions ahead of the relevant repository's `0.1`
release; details and process will be published as part of that
milestone work. Until then, the GitHub commit-via-PR flow constitutes
acceptance of the project licence for the contributed change.

## Where to ask

- **Bugs / feature requests:** the relevant repository's GitHub issue
  tracker
- **Security issues:** see the repository's `SECURITY.md` (where
  present) for the responsible-disclosure path
- **General questions:** the relevant repository's issue tracker;
  conversational venues are intentionally not listed here so the
  canonical record stays on GitHub
