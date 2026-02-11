# Changelog

## [2026-02-10] — Star Wars Agent Personality Feature

### 🆕 New Features
- **.vscode/skills/star-wars-agent-personality/SKILL.md**: Add Star Wars Agent Personality skill that assigns character personalities (Yoda, Han Solo, C-3PO, etc.) to spawned subagents
- **.github/prompts/enable-star-wars-agents.prompt.md**: Add prompt to activate Star Wars character personalities for all subagents

### 📝 Documentation
- **README.md**: Update project structure to include new Star Wars skill and prompt
- **README.md**: Expand Copilot Skills section to document both skills
- **README.md**: Add enable-star-wars-agents to prompts table
- **.github/copilot-instructions.md**: Add Star Wars skill and prompt to File Conventions table

---


## [2026-02-10] — Changes `65b66d8` to `b3855fc`

### 🆕 New Features
- feat: add README changelog generator skill with prompts, instructions, and CI workflow

### 📦 Other
- Merge pull request #2 from dc995/feat/readme-changelog-generator

<details><summary>Files changed</summary>

```
 .github/copilot-instructions.md                    |  39 +++++++
 .../instructions/changelog-format.instructions.md  |  27 +++++
 .github/instructions/readme-update.instructions.md |  24 +++++
 .github/prompts/generate-change-readme.prompt.md   |  66 ++++++++++++
 .github/prompts/generate-full-readme.prompt.md     |  39 +++++++
 .github/prompts/summarize-changes.prompt.md        |  31 ++++++
 .github/workflows/auto-readme.yml                  | 112 +++++++++++++++++++++
 .vscode/skills/readme-changelog-generator/SKILL.md |  98 ++++++++++++++++++
 CHANGELOG.md                                       |  18 ++++
 README.md                                          |  86 ++++++++++++++++
 10 files changed, 540 insertions(+)
```
</details>

---



## [2026-02-10] — Initial setup

### 🆕 New Features
- **README.md**: Add project README with structure, usage, and contributing guide.
- **.vscode/skills/readme-changelog-generator/SKILL.md**: Add Copilot skill for automated changelog generation.
- **.github/prompts/generate-change-readme.prompt.md**: Add prompt to generate changelog from recent changes.
- **.github/prompts/summarize-changes.prompt.md**: Add prompt to summarize changes since last entry.
- **.github/prompts/generate-full-readme.prompt.md**: Add prompt to generate a full README.

### ⚙️ Configuration
- **.github/copilot-instructions.md**: Add global Copilot instructions for the repo.
- **.github/instructions/changelog-format.instructions.md**: Add changelog formatting rules.
- **.github/instructions/readme-update.instructions.md**: Add README update rules.
- **.github/workflows/auto-readme.yml**: Add GitHub Action for automatic changelog generation on push.

---
