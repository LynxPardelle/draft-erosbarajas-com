# Draft: erosbarajas.com

Sanitized public source for the Zoolanding draft at `drafts/erosbarajas.com`.

## Start Here

| Task | Source |
| --- | --- |
| Safety, workflow, and closeout | [AGENTS.md](AGENTS.md) |
| Domain, environments, and required GitHub variables | [draft-repo.config.json](draft-repo.config.json) |
| Routes, canonical origin, and runtime settings | [site-config.json](site-config.json) |
| Page content | `{pageId}/page-config.json`, `{pageId}/components.json`, `{pageId}/variables.json`, and `{pageId}/i18n/` |
| Deployment implementation | [tools/deploy-draft.mjs](tools/deploy-draft.mjs) and [.github/workflows/](.github/workflows/) |
| Repository chronology | [changelog/README.md](changelog/README.md) |

Shared authoring, safety, asset, and alias guidance lives in the [Zoolandingpage documentation hub](https://github.com/LynxPardelle/zoolandingpage/blob/main/docs/README.md).

## Domain And Release Contract

The [fleet registry](https://github.com/LynxPardelle/zoolandingpage/blob/main/docs/drafts-registry.json) verifies `erosbarajas.com` as this repository's canonical domain. Registry version 1 has no production- or test-alias fields, so it does not authorize either kind of alias. `site-config.json` currently declares an empty alias list.

Work lands on `dev`; it does not deploy. Separate merged pull requests promote `dev -> test -> main`. GitHub Actions use OIDC; do not add long-lived AWS credentials.

Local-only notes, findings, logs, environment files, private keys, databases, PDFs, private photos, and agent state remain ignored. Documentation-only changes do not require visual QA; payload or rendered changes do.
