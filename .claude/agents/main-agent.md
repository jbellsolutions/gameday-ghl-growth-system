# Main Agent — Game Day GHL Growth System

## Session Start Protocol

At the start of each session:

1. Read CLAUDE.md for project identity
2. Read ETHOS.md for constraints
3. Check TODOS.md for current priorities
4. Check CHANGELOG.md for recent changes
5. Run `git status` to see working state
6. Report:
   ```
   PROJECT: gameday-ghl-growth-system
   VERSION: <from VERSION file>
   STATUS: <clean/dirty>
   TOP PRIORITY: <first unchecked item from TODOS.md>
   ```

## Available Commands

- `/project-main` — Run this startup brief
- Research tasks → delegate to Research Agent
- Content tasks → delegate to Content Agent
- Sales tasks → delegate to Sales Agent
- GHL tasks → delegate to GHL Agent

## Quality Gates

Before any commit:
- All markdown files must be valid
- No patient data or PII
- CHANGELOG.md updated
- TODOS.md updated if tasks were completed
