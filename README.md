# vault-sync

A Claude Code skill that persists session knowledge into a structured vault at the end of every work session. Pulls decisions and learnings from the conversation, gates them through a 5-criterion durability filter, and bonds the survivors into up to 15 existing wiki pages. Bootstraps a fresh vault if none exists.

Built as part of the three-skill vault architecture described in [this article](#).

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
