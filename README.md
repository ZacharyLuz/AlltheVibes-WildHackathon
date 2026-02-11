# AlltheVibes-WildHackathon

Automated documentation engine that keeps your README and CHANGELOG in sync with every change in the repo — powered by GitHub Copilot skills, prompts, and GitHub Actions.

## Quick Start

1. **Clone the repo:**
   ```bash
   git clone https://github.com/shyamsridhar123/AlltheVibes-WildHackathon.git
   cd AlltheVibes-WildHackathon
   ```

2. **Make changes** to any file in the repo.

3. **Generate documentation** using one of these methods:

   - **Copilot Prompt (recommended):** Open the command palette, run the `generate-change-readme` prompt, and Copilot will analyze your changes and update the changelog.
   
   - **Automatic (on push):** Push to `main` and the GitHub Action will auto-generate a changelog entry.

## Project Structure

```
AlltheVibes-WildHackathon/
├── .github/
│   ├── copilot-instructions.md          # Global Copilot behavior rules
│   ├── instructions/
│   │   ├── changelog-format.instructions.md  # Changelog formatting rules
│   │   └── readme-update.instructions.md     # README update rules
│   ├── prompts/
│   │   ├── enable-star-wars-agents.prompt.md # Enable Star Wars agent personalities
│   │   ├── generate-change-readme.prompt.md  # Generate changelog from changes
│   │   ├── generate-full-readme.prompt.md    # Generate a full README
│   │   └── summarize-changes.prompt.md       # Summarize changes since last entry
│   └── workflows/
│       └── auto-readme.yml                   # GitHub Action for auto-changelog
├── .vscode/
│   └── skills/
│       ├── readme-changelog-generator/
│       │   └── SKILL.md                      # Changelog generation skill
│       └── star-wars-agent-personality/
│           └── SKILL.md                      # Star Wars personality skill
├── CHANGELOG.md                              # Auto-generated changelog
├── README.md                                 # This file
├── swarm_mascot.py                           # ASCII art mascot
└── vibe_oracle.py                            # Chaotic vibe generator
```

## How It Works

### Copilot Skills

#### README/Changelog Generator
The skill in `.vscode/skills/readme-changelog-generator/SKILL.md` teaches Copilot how to:
- Analyze git diffs and commit messages
- Classify changes into categories (Features, Fixes, Refactors, etc.)
- Generate structured changelog entries
- Update the README

#### Star Wars Agent Personality
The skill in `.vscode/skills/star-wars-agent-personality/SKILL.md` teaches Copilot how to:
- Assign Star Wars character personalities to spawned subagents
- Inject character-specific communication styles (Yoda, Han Solo, C-3PO, etc.)
- Maintain technical accuracy while adding personality to agent interactions
- Keep each agent in character throughout their entire execution

### Prompts
| Prompt | What It Does |
|--------|-------------|
| `generate-change-readme` | Analyzes recent commits and generates a changelog entry |
| `summarize-changes` | Finds all changes since the last changelog entry |
| `generate-full-readme` | Creates a complete README from the current repo state |
| `enable-star-wars-agents` | Activates Star Wars character personalities for all subagents |

### Instructions
| File | Scope |
|------|-------|
| `copilot-instructions.md` | Global rules for all Copilot interactions in this repo |
| `changelog-format.instructions.md` | Formatting rules applied when editing CHANGELOG.md |
| `readme-update.instructions.md` | Rules applied when editing README.md |

### GitHub Action
On every push to `main`, the workflow:
1. Reads the commit messages and diff
2. Categorizes changes using conventional commit prefixes
3. Generates a changelog entry with date and commit range
4. Prepends it to `CHANGELOG.md`
5. Commits and pushes the update

## Recent Changes

See [CHANGELOG.md](CHANGELOG.md) for a full history of changes.

## Contributing

1. Use [Conventional Commits](https://www.conventionalcommits.org/) for commit messages.
2. After making changes, run the `generate-change-readme` Copilot prompt to update docs.
3. The GitHub Action will also auto-update on push to `main`.

## License

MIT
