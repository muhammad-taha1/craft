# craft

A Claude Code plugin that encodes a coherent software engineering philosophy into your workflow.

## Install

**Claude Code plugin marketplace:**

```
/plugin marketplace add thisistaha/craft
/plugin install craft@craft
```

Then `/reload-plugins` if needed. Skills are namespaced: `/craft:principles`, `/craft:discover`, etc.

**Any agent via [`npx skills`](https://github.com/vercel-labs/skills):**

```bash
# all five skills
npx skills add thisistaha/craft

# a single skill
npx skills add thisistaha/craft --skill principles

# globally, to Claude Code only
npx skills add thisistaha/craft -a claude-code -g
```

## What's inside

Five skills — see [`plugins/craft/README.md`](plugins/craft/README.md) for details.

## Development

```bash
# Test locally without installing
claude --plugin-dir ./plugins/craft

# Validate before pushing
claude plugin validate
```

## License

MIT
