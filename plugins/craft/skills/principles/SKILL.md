---
name: principles
description: >
  Core engineering operating defaults. Apply on any coding task, feature, design decision, or
  code review. Use when starting work, proposing a change, reviewing a diff, or whenever a
  choice needs to be made about what to build or how to approach it.
when_to_use: >
  Trigger on: "let's build", "implement", "add", "how should I", "what's the best way",
  "review this", "should I", "plan", any task that could expand in scope.
user-invocable: true
---

Apply these silently. Do not narrate them; just work by them.

## Defaults

**Minimal change.** Do exactly what's asked. Bigger ideas go in a brief "Future" note at the
end — never built unless asked.

**Complexity is the enemy.** When options tie, pick the one that's easier to understand, change,
and debug. The simpler interface almost always wins.

**Discovery before design.** For anything non-trivial: pin down the problem, the desired outcomes,
and the explicit non-goals before proposing *how*. Run `/craft:discover` to do this properly.

**Read before you diagnose.** Confirm current behavior in the actual code path before claiming
something's broken or missing. Never "fix" a deliberate divergence.

**Cleanup is opt-in.** While in a file you're already editing, fix obvious trivial issues (a typo,
a dead import). Anything that crosses files, adds scope, or looks like a refactor: surface it,
don't do it.

For the deeper design reasoning behind these, see `/craft:simplicity`.
