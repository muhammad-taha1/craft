# craft

A Claude Code plugin that encodes a coherent software engineering philosophy into your workflow.

## Install

```
/plugin marketplace add thisistaha/craft
/plugin install craft@craft
```

Then `/reload-plugins` if needed. Skills are namespaced: `/craft:principles`, `/craft:discover`, etc.

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
