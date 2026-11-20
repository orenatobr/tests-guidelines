# tests-guidelines

A test-first workflow for new features, bug fixes and refactors, with 80% or higher coverage across unit, integration and E2E tests. Adapted from the `tdd-workflow` skill in affaan-m/everything-claude-code (MIT), see `NOTICE.md`.

## Install

For Claude Code, copy the skill folders into your personal skills directory:

```bash
git clone https://github.com/orenatobr/tests-guidelines.git
mkdir -p ~/.claude/skills
cp -R tests-guidelines/skills/* ~/.claude/skills/
```

Start a new Claude Code session. Skills load from the `description` in each `SKILL.md`, so they trigger on their own and can also be called by name.

Other agents: each skill is a folder with a `SKILL.md` (YAML frontmatter plus Markdown). Tools that read the Agent Skills format can load `skills/` as it is. For the rest, paste the body of the `SKILL.md` into the agent's instruction file.

## Usage

Invoke `/tests-guidelines` when writing tests or doing TDD. It also triggers on "coverage", "unit test" and "integration test".

## Requirements

Nothing beyond an agent that loads skills.

## Related skills

`programming-best-practices` defers to this skill for every test decision.

## What is in this repo

| Path | Purpose |
|------|---------|
| `skills/tests-guidelines/` | The `tests-guidelines` skill. |
| `CHANGELOG.md` | Notable changes, in Keep a Changelog format. |
| `AGENTS.md` | Rules for AI agents that edit this repo. |

## Contributing

`main` is protected: changes land through a pull request with one approval. See [AGENTS.md](AGENTS.md) for the conventions.

## License

MIT, see [LICENSE](LICENSE).
Third-party material is credited in [NOTICE.md](NOTICE.md).

