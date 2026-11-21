# Tresor — Beta Releases

> **Experimental beta software · Not production-ready**
>
> Tresor is a Windows-first, offline file-vault project under active development.
> Releases in this repository are **for technical evaluation and testing only**.
> They are **not certified, independently security-audited, or approved for production use**.
> **Do not rely on these builds to protect sensitive, confidential, valuable, or irreplaceable data.**
> Use only disposable sample files and keep independent backups.

## Release status

| Item | Current status |
| --- | --- |
| Software maturity | **Experimental beta / test build** |
| Distribution | Windows desktop test packages and update-feed artifacts |
| Latest **publicly published** beta verified on 2026-11-21 | `v0.1.1-beta.12` |
| `v0.1.1-beta.13` | Prepared in the private source repository; **not confirmed as a publicly published release** |
| Stable / production release | **Not available** |
| Support, compatibility and data-recovery guarantees | **None** |

**Release availability matters:** A version mentioned in a changelog or source tag does not mean it is publicly available or approved for use. GitHub draft releases and unpublished artifacts are not general releases.

[View published test releases](https://github.com/rootkid-code/tresor-releases/releases)

## What Tresor is testing

Tresor explores a local-first encrypted file vault with a native Windows desktop host (Tauri/Rust) and a React/TypeScript interface. The source project's current beta scope includes:

- Vault creation and passphrase-based unlock, with key-management and encrypted storage primitives.
- Encrypted file import, metadata search, previews, and explicitly initiated export.
- Separate encrypted sharing packages, backup and recovery workflows.
- Desktop session protection and experimental packaging/updater infrastructure.

These are **implemented or documented beta capabilities**, not guarantees of correct operation under every condition or proof of security.

## Known limitations and work remaining

The project needs substantial additional engineering and verification before a stable release:

1. **Independent security assessment:** review the threat model, cryptography integration, file-system trust boundaries, dependencies and desktop attack surface; remediate findings.
2. **Rollback resistance:** the internal committed-state verification exists, but a reliable **external monotonic anti-rollback anchor is still missing**. Rolling back an entire vault to an older consistent state is not fully covered.
3. **Recovery assurance:** broaden destructive-failure, interrupted-write, corrupt-file, migration, backup/restore and cross-version tests; verify restore procedures using disposable vaults.
4. **Windows compatibility and usability:** expand real-device testing across supported Windows configurations, WebView2 environments, high-DPI displays and accessibility scenarios.
5. **Release integrity:** verify installer signing, updater signing and provenance on each build; test installation, upgrade, rollback and uninstall with repeatable evidence.
6. **Performance and optional features:** continue evaluating resource usage, preview behavior and opt-in local super-resolution without treating experimental modules as production-stable.
7. **Operational readiness:** finalize documentation, vulnerability reporting, support expectations, release criteria and reproducible acceptance evidence.

**Security model boundary:** Tresor does not promise protection against a compromised operating system, privileged malware, hardware keyloggers, or all RAM, paging and screen-capture exposure. A beta test is not a substitute for established storage and backup solutions.

## If you choose to test a beta

- Use **non-sensitive, disposable sample files only**. Do not import credentials, confidential documents, unique photos or your only copy of any file.
- Use a dedicated test vault and keep independent copies outside Tresor.
- Download artifacts only from the [GitHub Releases page](https://github.com/rootkid-code/tresor-releases/releases).
- Where provided, compare downloaded files with the accompanying `SHA256SUMS.txt`. Checksums help detect accidental changes, but **do not establish trust in the publisher by themselves**.
- Do not assume that draft assets, updater metadata or installer signatures imply a completed security review.
- Expect breaking changes, defects, possible data loss and incompatible beta formats.

## Release process

The source project uses a controlled, tag-based Windows packaging workflow. Build artifacts and checksums are generated as release candidates; publication is a separate manual review step. The public repository hosts distribution assets and an updater feed where available.

**A published beta is still a beta.** Publication does not signify production readiness or a security certification.

## Project links

- [Public beta downloads](https://github.com/rootkid-code/tresor-releases/releases)
- [Source repository](https://github.com/rootkid-code/tresor) *(may require access; currently private)*
- [Release notes](https://github.com/rootkid-code/tresor/releases) *(source-repository access may be required)*

---

### Development status / disclaimer

**Tresor is a development and test project, not a finished or production-ready product.** Important security, quality-assurance, resilience, compatibility, release and documentation work remains. No warranty of data integrity, data recovery or confidentiality is made for these beta builds. Please do not use them for real-world secure storage.
