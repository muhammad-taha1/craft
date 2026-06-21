# craft plugin

Five skills that encode a coherent software engineering philosophy into your Claude Code sessions.

| Skill | Invocation | Trigger |
| :-- | :-- | :-- |
| `principles` | `/craft:principles` | Any coding task — operating defaults, scope discipline, complexity mindset |
| `discover` | `/craft:discover [idea]` | Before designing — requirements interview, produces a brief |
| `simplicity` | `/craft:simplicity` | Design decisions — deep modules, abstraction layers, Rule of Three |
| `domain-modeling` | `/craft:domain-modeling` | Backend architecture, modeling, DDD strategic/tactical patterns |
| `testing` | `/craft:testing` | Writing tests — interface-seam TDD, no internal mocking, SRP |

Skills auto-trigger based on context. You can also invoke any of them directly.

## Philosophy

- **Complexity is the enemy.** Judge every change by how much harder it makes the system to understand, change, and debug.
- **Deep modules over shallow ones.** A simple interface hiding powerful implementation beats many small pass-through classes.
- **Discovery before design.** Pin down the problem, outcomes, and non-goals before proposing a solution.
- **Minimal change / YAGNI.** Do exactly what's asked. Surface bigger ideas as future notes; don't build them.
- **DDD, tiered.** Ubiquitous language and bounded contexts everywhere. Aggregates, events, and ACL only when complexity earns them.
- **TDD at the seam.** Test what the interface promises, not every internal method.

Sources: *A Philosophy of Software Design* (Ousterhout), *Domain-Driven Design* (Evans), *Extreme Programming* (Beck).

## Optional: always-on defaults for your own machine

The `principles` skill description stays in context for you automatically, but for the strongest
always-on effect, add one line to your `~/.claude/CLAUDE.md`:

```
At the start of any coding task, apply the craft:principles operating defaults.
```

This references, not duplicates, the skill — single source of truth stays in the plugin.
