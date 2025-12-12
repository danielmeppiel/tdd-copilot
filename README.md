# TDD Copilot 🔴🟢🔵

[![Install with APM](https://img.shields.io/badge/📦_Install_with-APM-blue?style=flat-square)](https://github.com/danielmeppiel/apm)

**Test-Driven Development workflow encoded as VSCode agent handoffs.**

Red → Green → Refactor, guided by AI.

## Quick Start

```bash
apm install danielmeppiel/tdd-copilot
apm compile
```

Then in VSCode Copilot Chat:

```
@tdd-red Add email validation to the User class
```

## The Flow

```
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│   🔴 RED        │────▶│   🟢 GREEN      │────▶│   🔵 REFACTOR   │
│   @tdd-red      │     │   @tdd-green    │     │   @tdd-refactor │
│                 │     │                 │     │                 │
│ Write failing   │     │ Make tests      │     │ Clean up code   │
│ tests first     │     │ pass            │     │ keep tests green│
└─────────────────┘     └─────────────────┘     └─────────────────┘
      Handoff:               Handoff:
   "Make Tests Pass"      "Improve Code"
```

## Agents

| Agent | What it does | Tools |
|-------|--------------|-------|
| `@tdd-red` | Writes failing tests based on your feature description | Read-only (no edits) |
| `@tdd-green` | Implements minimum code to make tests pass | Full editing |
| `@tdd-refactor` | Refactors code while ensuring tests stay green | Full editing |

## Why Use This?

- **Encode your methodology**: TDD discipline, automated
- **Guided workflow**: Handoff buttons prevent skipping steps
- **Shareable**: One `apm install` for your whole team
- **IDE-native**: Works directly in VSCode Copilot Chat

## Manual Installation

If you don't use APM, copy `.apm/agents/*.agent.md` to your project's `.github/agents/` folder.

## License

MIT
