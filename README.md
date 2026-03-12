# agent-quality-skills

Consolidated skill files for AI coding agents. Four skills distilled from [citypaul/.dotfiles](https://github.com/citypaul/.dotfiles/tree/main/claude/.claude/skills) — ~83% reduction in tokens while retaining the core behavioural signal.

## Skills

| Skill | Description |
|---|---|
| [architecture](architecture/SKILL.md) | Functional style, TypeScript strict mode, DDD, hexagonal architecture, repository pattern |
| [testing](testing/SKILL.md) | TDD workflow, behavior-driven tests, factory pattern, coverage, refactoring, mutation testing |
| [process](process/SKILL.md) | Incremental planning, plan files, PR discipline, documentation, CI debugging |
| [review](review/SKILL.md) | Test quality scoring using Dave Farley's 8 properties (Farley Score) |

## Usage

Load the relevant skill(s) into your agent's context at the start of a task. Skills are designed to be loaded selectively — load `testing` for TDD work, `architecture` for design decisions, `review` for test suite analysis, `process` for planning and CI work.
