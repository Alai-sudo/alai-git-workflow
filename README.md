# alai-git-workflow

A Claude Code Skill that enforces Git collaboration best practices using the `dev/alai-sudo` branch.

## What It Does

When installed, Claude Code will automatically:

- Create and work on `dev/alai-sudo` branch instead of main/master
- Follow atomic commit practices with clear commit messages
- Use conventional commit format (`feat:`, `fix:`, `refactor:`, etc.)
- Push changes to remote and create PRs when ready

## Installation

### Step 1: Add Marketplace Source

In Claude Code, run:

```
/plugin marketplace add Alai-sudo/alai-git-workflow
```

### Step 2: Install the Skill

```
/plugin install alai-git-workflow@alai-skills
```

## Usage

Once installed, the skill activates automatically when you work on coding tasks. Claude will:

1. Switch to `dev/alai-sudo` branch before making changes
2. Commit with descriptive messages following conventional format
3. Push and create PRs when you're ready

## Uninstall

```
/plugin uninstall alai-git-workflow@alai-skills
/plugin marketplace remove alai-skills
```

## License

MIT
