# TDD Copilot

This package provides a Test-Driven Development workflow using VSCode agent handoffs.

## Agents

| Agent | Purpose | Handoff |
|-------|---------|--------|
| `@tdd-red` | Write failing tests first | → `@tdd-green` |
| `@tdd-green` | Implement minimum code to pass | → `@tdd-refactor` |
| `@tdd-refactor` | Clean up while keeping tests green | (complete) |

## Usage

1. Start with `@tdd-red` and describe the feature you want
2. Agent writes failing tests
3. Click **"Make Tests Pass"** handoff button
4. Agent implements minimum code
5. Click **"Improve Code"** handoff button
6. Agent refactors while keeping tests green

## Installation

```bash
apm install danielmeppiel/tdd-copilot
apm compile
```
