# /s — shorten the last response

A one-letter [Agent Skill](https://agentskills.io). Type `/s` when your coding agent's answer is too long to read, and it rewrites it keeping only what matters.

## Install

Any agent (Claude Code, Codex, Cursor, Gemini CLI, GitHub Copilot, OpenCode and [more](https://github.com/vercel-labs/skills/blob/main/docs/agents.md)):

```bash
npx skills add yakovlef/skill-s -g
```

Claude Code only, no Node required:

```bash
curl -fsSL https://raw.githubusercontent.com/yakovlef/skill-s/main/skills/s/SKILL.md --create-dirs -o ~/.claude/skills/s/SKILL.md
```

Start a new session, then type `/s`. Add a hint to steer it: `/s one sentence`, `/s only the risks`.

## Why

- **One letter.** Fast to type right after a wall of text.
- **Zero context cost in Claude Code.** `disable-model-invocation: true` keeps it out of the model's skill list, so it never fires on its own and adds no tokens to your sessions.
- **Tiny.** Read the whole thing in [SKILL.md](skills/s/SKILL.md) and tweak it to taste.

## Uninstall

```bash
npx skills remove s -g
```

## License

[MIT](LICENSE)
