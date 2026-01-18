---
name: alai-git-workflow
description: Git collaboration workflow for alai-sudo. Use this skill when working on any coding task that involves file changes. Enforces creating and using the dev/alai-sudo branch, following Git collaboration best practices including clear commit messages and avoiding direct commits to main branch.
---

# Alai Git Workflow

## Core Principle

Always work on a dedicated branch `dev/alai-sudo` instead of main/master.

## Workflow

### Before Starting Work

1. Check current branch status
2. Create or switch to `dev/alai-sudo` branch:
   ```bash
   git checkout -b dev/alai-sudo || git checkout dev/alai-sudo
   ```

### During Work

- Make atomic commits with clear, descriptive messages
- Keep commits focused on single logical changes
- Never commit directly to main/master

### Commit Message Format

```
<type>: <short description>

[optional body explaining why]
```

Types: `feat`, `fix`, `refactor`, `docs`, `test`, `chore`

### After Completing Work

1. Ensure all changes are committed
2. Push to remote: `git push -u origin dev/alai-sudo`
3. Create PR when ready for review

## Branch Naming

- Development branch: `dev/alai-sudo`
- Feature branches (if needed): `dev/alai-sudo/<feature-name>`
