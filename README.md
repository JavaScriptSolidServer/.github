# JavaScript Solid Server (JSS) Org

The agentic-native, Nostr-aligned, standards-track home for Solid pod
infrastructure and tooling.

## Featured projects

- **[JSS][jss]** — A minimal, fast, JSON-LD-native Solid server. ESM,
  no native modules, runs on Termux, postmarketOS, and Cloudflare
  Workers.
- **[jss-git][jss-git]** — Web-based git browser for Solid pods (Preact
  + isomorphic-git, no build step).
- **[podkey][podkey]** — Nostr-key browser extension for NIP-98
  authentication against Solid pods.
- **[jss-android][jss-android]** — Native Android pod (work in
  progress).
- **[git-credential-nostr][gcn]** — Git helper for Nostr-signed
  commits.
- **[nostr-git-sync][ngs]** — Sync git repositories over Nostr relays.

## Standards alignment

- W3C [CID v1.0][cid] — Recommendation. Implemented in JSS pod
  profiles.
- `did:nostr` — Registered DID method. Native resolution in JSS.
- W3C [LWS][lws] (Linked Web Storage) — FPWD; JSS implements
  ahead of REC.
- AGPL-3.0 across all projects.

## Get involved

See [CONTRIBUTING][contrib] for workflow, code style, AI-assistance
disclosure, and fork-policy expectations.

[jss]: https://github.com/JavaScriptSolidServer/JavaScriptSolidServer
[jss-git]: https://github.com/JavaScriptSolidServer/git
[podkey]: https://github.com/JavaScriptSolidServer/podkey
[jss-android]: https://github.com/JavaScriptSolidServer/jss-android
[gcn]: https://github.com/JavaScriptSolidServer/git-credential-nostr
[ngs]: https://github.com/JavaScriptSolidServer/nostr-git-sync
[cid]: https://www.w3.org/TR/cid-1.0/
[lws]: https://www.w3.org/TR/2026/WD-lws10-authn-ssi-cid-20260423/
[contrib]: ./CONTRIBUTING.md
