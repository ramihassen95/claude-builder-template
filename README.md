# Claude Builder Template

Reusable Claude Code builder skills based on [Superpowers](https://github.com/obra/superpowers) by Jesse Vincent.

## What's Included

| Skill | Purpose |
|-------|--------|
| `brainstorming` | Refine ideas into specs through questions |
| `writing-plans` | Create detailed implementation plans |
| `executing-plans` | Batch execution with checkpoints |
| `subagent-driven-development` | Fresh subagent per task + two-stage review |
| `test-driven-development` | RED-GREEN-REFACTOR cycle enforcement |
| `systematic-debugging` | 4-phase root cause analysis |
| `using-git-worktrees` | Isolated development branches |
| `verification-before-completion` | Evidence before claims |
| `requesting-code-review` | Code review dispatch |
| `receiving-code-review` | Handle review feedback |
| `dispatching-parallel-agents` | Concurrent subagent workflows |
| `finishing-a-development-branch` | Merge/PR decision workflow |
| `using-superpowers` | Meta-skill for skill discovery |
| `writing-skills` | Create new skills (TDD for docs) |

## Installation

### Copy to Any Project

```bash
# Clone this template
git clone https://github.com/ramihassen95/claude-builder-template.git temp-skills

# Copy skills to your project
cp -r temp-skills/.claude/skills/builder/* your-project/.claude/skills/builder/

# Clean up
rm -rf temp-skills
```

### Add to CLAUDE.md

Add this to your project's `CLAUDE.md`:

```markdown
## Builder Workflow

When building features:
1. Use `brainstorming` skill to refine requirements
2. Use `writing-plans` skill to create implementation plan
3. Use `subagent-driven-development` or `executing-plans` to implement
4. Use `verification-before-completion` before claiming done
5. Use `finishing-a-development-branch` to complete

All implementation follows `test-driven-development` skill.
```

## Philosophy

- **Test-Driven Development** - Write tests first, always
- **Systematic over ad-hoc** - Process over guessing  
- **Complexity reduction** - Simplicity as primary goal
- **Evidence over claims** - Verify before declaring success
- **YAGNI** - You Aren't Gonna Need It

## Credits

Based on [Superpowers](https://github.com/obra/superpowers) by [Jesse Vincent](https://github.com/obra).

MIT License
