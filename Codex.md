# Compatibility Pointer

Start with [AGENTS.md](AGENTS.md), then use [README.md](README.md) as the task index.

Durable repository decisions:

- Canonical domain: `erosbarajas.com`. The fleet registry does not define production or test aliases; do not invent them.
- Release path: `dev -> test -> main`; only `test` and `main` deploy.
- Runtime truth: [site-config.json](site-config.json) and task-specific page JSON.
- Chronology: [changelog/README.md](changelog/README.md).

Do not add implementation history or local investigation here.
