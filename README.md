# vault-sync

A Claude Code skill that persists session knowledge into a structured vault at the end of every work session. Pulls decisions and learnings from the conversation, gates them through a 5-criterion durability filter, and bonds the survivors into up to 15 existing wiki pages. Bootstraps a fresh vault if none exists.


## Part of vault-toolkit

This is one of three skills designed to work together as a system. The trio shares a manifest schema and a vault-index hash chain. **Installing this skill standalone without the other two will produce runtime errors** — `vault-lint` expects a manifest written by `vault-restructure`; `vault-sync` expects either to bootstrap a vault itself or to find one scaffolded by `vault-restructure`.

**Recommended install:** the [`vault-toolkit` plugin](https://github.com/17july1997-cpu/vault-toolkit) bundles all three skills with verified compatibility in a single Claude Code plugin install.

Sibling repos:
- [vault-restructure](https://github.com/17july1997-cpu/vault-restructure) — file routing + manifest creation
- [vault-sync](https://github.com/17july1997-cpu/vault-sync) — vault bootstrap + session ingestion
- [vault-lint](https://github.com/17july1997-cpu/vault-lint) — three-tier health checks

This repo is retained for code inspection, cherry-picking, and individual-skill forking.

## Install

Clone into your Claude Code skills folder:

    cd ~/.claude/skills
    git clone https://github.com/17july1997-cpu/vault-sync.git

Then in Claude Code, type `/vault-sync` at the end of any session.

## How it works

See [SKILL.md](SKILL.md) for the full specification, and [references/](references/) for deep documentation.

## Related skills

- [vault-restructure](https://github.com/17july1997-cpu/vault-restructure) — normalize a folder dump into a routed vault
- [vault-lint](https://github.com/17july1997-cpu/vault-lint) — read-only audit of vault drift

## License

MIT. Fork it, make it yours.
