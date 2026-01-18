# alai-git-workflow

A Claude Code Skill that enforces Git collaboration best practices using the `dev/alai-sudo` branch.

## What It Does

When installed, Claude Code will automatically:

- Create and work on `dev/alai-sudo` branch instead of main/master
- Follow atomic commit practices with clear commit messages
- Use conventional commit format (`feat:`, `fix:`, `refactor:`, etc.)
- Push changes to remote and create PRs when ready

## Installation

### Option 1: Download .skill file

1. Download `alai-git-workflow.skill` from [Releases](https://github.com/Alai-sudo/alai-git-workflow/releases)
2. Place it in `~/.claude/skills/`

### Option 2: Clone and install

```bash
git clone https://github.com/Alai-sudo/alai-git-workflow.git
cp alai-git-workflow/SKILL.md ~/.claude/skills/alai-git-workflow/
```

### Option 3: Add to Claude Code settings

Add to your `~/.claude/settings.json`:

```json
{
  "skills": [
    "https://github.com/Alai-sudo/alai-git-workflow"
  ]
}
```

## Usage

Once installed, the skill activates automatically when you work on coding tasks. Claude will:

1. Switch to `dev/alai-sudo` branch before making changes
2. Commit with descriptive messages following conventional format
3. Push and create PRs when you're ready

## License

MIT
