# .github

Default community files for the AuraSpeak organization: profile, contribution guidelines, and (when added) issue/PR templates and workflows.

---

## What is AuraSpeak?

AuraSpeak is an alternative to Discord and Teamspeak. Security and openness are the main focus; the aim is to keep the project free once released. Decentralization and security through encryption are central.

The project is not yet in alpha or beta and is far from release. Expect breaking changes and rapid iteration.

---

## Repositories

**Main repo (public):** [AuraSpeak/auraspeak](https://github.com/AuraSpeak/auraspeak) – project overview, docs, roadmap, ADRs.

| Repo | Role |
|------|------|
| [workflow](https://github.com/AuraSpeak/workflow) | Unified local dev setup: clone repos, Go workspace, bootstrap, test-all. |
| [debug-ui](https://github.com/AuraSpeak/debug-ui) | Web interface for inspecting packet flow; Go backend, Vue frontend. |
| [client](https://github.com/AuraSpeak/client) | AuraSpeak desktop client; highly decoupled, testable in isolation or in the debug UI. |
| [server](https://github.com/AuraSpeak/server) | Community server code; packet handling, broadcast, lifecycle. |
| [protocol](https://github.com/AuraSpeak/protocol) | Application-level protocol (framing, packet types) over UDP/DTLS. |
| [network](https://github.com/AuraSpeak/network) | DTLS-UDP transport, readloop, packet router; used by client and server. |

---

## What's in this repo

This README (organization profile), [CONTRIBUTING.md](CONTRIBUTING.md) (contribution guidelines), [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) (code of conduct), [SECURITY.md](SECURITY.md) (security policy), and issue templates (bug report, feature request, question). Optionally in the future: pull request template, GitHub Actions workflows.

---

## Quickstart

For local development, clone the workflow repo and run setup and bootstrap:

```bash
git clone https://github.com/AuraSpeak/workflow
cd workflow
just setup
just bootstrap
```

Use the [justfile](https://github.com/AuraSpeak/workflow/blob/main/justfile) in the workflow repo (`just setup`, `just bootstrap`, `just test-all`, etc.).

---

## Links

- **Main repo:** [AuraSpeak/auraspeak](https://github.com/AuraSpeak/auraspeak) (public) – docs, roadmap, architecture.
- **Blog:** [auraspeak.github.io](https://auraspeak.github.io).
- **Dev setup:** [AuraSpeak/workflow](https://github.com/AuraSpeak/workflow) – see Quickstart above.
