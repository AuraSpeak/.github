# Contributing to AuraSpeak

Thanks for your interest in contributing. AuraSpeak is in pre-alpha; expect breaking changes and rapid iteration.

---

## Before you start

- **Main repo:** [AuraSpeak/auraspeak](https://github.com/AuraSpeak/auraspeak) – docs, roadmap, architecture.
- **Status:** Pre-alpha. Breaking changes are possible.

---

## Dev setup

Local development runs through [AuraSpeak/workflow](https://github.com/AuraSpeak/workflow).

1. Clone the workflow repo and run setup and bootstrap:

   ```bash
   git clone https://github.com/AuraSpeak/workflow
   cd workflow
   just setup
   just bootstrap
   ```

2. Useful commands (from the [justfile](https://github.com/AuraSpeak/workflow/blob/main/justfile)): `just setup`, `just bootstrap`, `just test-all`, `just clean`.

---

## Bugs and ideas

Open an issue in the repo that fits (e.g. protocol bug → protocol repo, general question → [auraspeak](https://github.com/AuraSpeak/auraspeak)).

- Describe what happens or what you expect.
- For bugs: include Go version and OS if relevant.

---

## Submitting changes (PRs)

1. Fork the repo, create a branch, make your changes.
2. Before opening a PR: if you work on protocol, network, client, server, or debug-ui, run `just test-all` from the workflow repo.
3. Open a PR against the default branch of the repo you changed.
4. Write a short description; link to an issue if one exists.

---

## Versioning

We use [SemVer](https://semver.org/):

| Type   | When to use |
|--------|-------------|
| **Major** | API or other breaking changes. |
| **Minor** | New features or small additions (e.g. new packet type). |
| **Patch** | Bugfixes without API changes. |

---

## Code and style

- Go: use `gofmt`, sensible names, usual conventions.
- No long style guide here; when in doubt, ask in an issue.

---

## License

By submitting a PR, you agree that your contributions are under the same license as the project (e.g. [workflow/LICENSE](https://github.com/AuraSpeak/workflow/blob/main/LICENSE)).
