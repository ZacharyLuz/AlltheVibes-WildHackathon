# AlltheVibes-WildHackathon

Python hackathon toolkit with two flavors: a fully local **Ollama** CLI agent and a set of **Azure OpenAI–powered mini-agents** for repo insights, reviews, and chaos visualizations.

```text
                          ╔══════════════════════════════════════════════════════╗
                          ║     🐝  A L L   T H E   V I B E S  🐝               ║
                          ║          A G E N T    S W A R M                      ║
                          ╚══════════════════════════════════════════════════════╝

       ┌─────────────────────────────────────────────────────────────────────────────────┐
       │                        🌐  G I T H U B   C O P I L O T                        │
       │                         M U L T I - A G E N T   S Y S T E M                   │
       │                                                                                 │
       │                              ┌─────────────┐                                    │
       │                              │  🤠  BETH   │                                    │
       │                              │ Orchestrator │                                    │
       │                              └──────┬──────┘                                    │
       │                   ┌────────┬────────┼────────┬─────────┐                        │
       │                   ▼        ▼        ▼        ▼         ▼                        │
       │             ┌──────────┐┌────────┐┌────────┐┌────────┐┌──────────┐              │
       │             │ 📋  PM   ││ 🔬 Re- ││ 🎨 UX  ││ 💻 Dev ││ 🧪 Test │              │
       │             │Strategist││searcher││Designer││Builder ││Enforcer │              │
       │             └──────────┘└────────┘└────────┘└────────┘└──────────┘              │
       │                                      │                                          │
       │                        ┌──────────────┼──────────────┐                           │
       │                        │              │              │                           │
       │                  ┌──────────┐   ┌──────────┐   ┌──────────┐                      │
       │                  │ 🛡️ Secur-│   │ 🧰 Mac-  │   │ 🦈 Shark │                      │
       │                  │  ity Rev.│   │  Gyver   │   │  bait    │                      │
       │                  └──────────┘   └──────────┘   └──────────┘                      │
       └─────────────────────────────────────────────────────────────────────────────────┘

       ┌─────────────────────────────────────────────────────────────────────────────────┐
       │                    🖥️   L O C A L   C L I   A G E N T S                        │
       │                          ( O l l a m a  P o w e r e d )                         │
       │                                                                                 │
       │    ┌──────────────┐      ┌───────────────────────────────────────────────┐       │
       │    │  🔀 ROUTER   │─────▶│  Agent Selection Based on User Intent        │       │
       │    │ Intent Class.│      └───────────────────────────────────────────────┘       │
       │    └──────┬───────┘                                                             │
       │           │  routes to:                                                         │
       │     ┌─────┼────────┬────────────┬─────────────┬──────────────┐                  │
       │     ▼     ▼        ▼            ▼             ▼              ▼                  │
       │  ┌──────┐┌──────┐┌───────────┐┌───────────┐┌────────────┐┌──────────┐          │
       │  │🤖    ││🔮    ││📊         ││🔍         ││🗄️          ││🔮        │          │
       │  │ Repo ││Commit││  Chaos    ││   Code    ││    SQL     ││  Vibe   │          │
       │  │Copil-││Whisp-││  Visual-  ││ Reviewer  ││ Generator  ││ Oracle  │          │
       │  │ ot   ││ erer ││  izer     ││           ││            ││         │          │
       │  └──────┘└──────┘└───────────┘└───────────┘└────────────┘└──────────┘          │
       │                                                                                 │
       │  ┌──────────────────────────────────────────────────────────────────────┐        │
       │  │  🛠️  TOOLS: calculator │ shell │ read/write │ web_search │ roast   │        │
       │  └──────────────────────────────────────────────────────────────────────┘        │
       └─────────────────────────────────────────────────────────────────────────────────┘

       ┌─────────────────────────────────────────────────────────────────────────────────┐
       │                 😂  C O M E D Y   A G E N T S  ( O p e n A I )                 │
       │                                                                                 │
       │         ┌──────────────────┐              ┌──────────────────┐                   │
       │         │  👨 DAD JOKES    │              │ 🚪 KNOCK KNOCK  │                   │
       │         │  "Hi Hungry,    │              │  "Who's there?"  │                   │
       │         │   I'm Dad!"    │              │  "Bug."          │                   │
       │         └──────────────────┘              │  "Bug who?"     │                   │
       │                                           │  "Bug in prod!" │                   │
       │                                           └──────────────────┘                   │
       └─────────────────────────────────────────────────────────────────────────────────┘

           \   /        \   /        \   /        \   /        \   /
       _.--'(  )'--._.--(  )'--._.--'(  )'--._.--(  )'--._.--'(  )'--._
      /  .-. \/ .-.  /.-. \/ .-.\/.-. \/ .-.\/.-. \/ .-.\/.-. \/ .-.  \
     | ( O ) () ( O )( O ) () ( O( O ) () ( O( O ) () ( O( O ) () ( O )|
      \  '-' /\ '-'  \'-' /\ '-'/\'-' /\ '-'/\'-' /\ '-'/\'-' /\ '-'  /
       '-.__(  )__.--'(  )'--.(  )__.-'(  )'--.(  )__.--'(  )'--.(  )_'
           /   \      /   \    /   \    /   \    /   \    /   \
         | PUSH! |  | VIBE! |  | CODE! | | SWARM |  | SHIP! |  | HACK! |
          '-----'    '-----'    '-----'   '-----'    '-----'    '-----'

                 🐝 THE SWARM IS ALIVE. PUSH YOUR CODE. TRUST THE VIBES. 🐝
```

## Quick Start

1) **Install dependencies**

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

2) **Run the local Ollama CLI agent (`agent.py`)**

- Install Ollama and pull a model (`ollama pull qwen2.5:7b`)
- Optional: adjust `OLLAMA_BASE_URL` / `OLLAMA_MODEL` in `.env`
- Start: `python agent.py`

3) **Run the Azure OpenAI utilities (`main.py`)**

- Export Azure settings: `ENDPOINT_URL`, `DEPLOYMENT_NAME`, `AZURE_OPENAI_API_VERSION` (and sign in with `az login` or a service principal so `DefaultAzureCredential` works)
- Try commands:
  - `python main.py router` (intent router demo)
  - `python main.py review path/to/file`
  - `python main.py whisper` (commit narrator)
  - `python main.py visualize` (git stats dashboard)
  - `python main.py sql "describe table foo"`

4) **Vibe extras (optional)**

- `python vibe_oracle.py "ask the oracle"` for chaotic prophecies
- `python swarm_chaos.py` / `python swarm_mascot.py` for swarm flair

## What it does

- **Local CLI agent (`agent.py` + `tools.py`)** — Ollama-backed chat loop with tools for shell commands, file read/write, math, datetime, web search, and roasting the agent roster.
- **Azure mini-agents (`main.py` + `agents/`)** — Router plus utilities powered by Azure OpenAI:
  - `repo_copilot` generates README drafts from repo context
  - `commit_whisperer` narrates recent git activity
  - `chaos_visualizer` renders contributor/history stats
  - `code_reviewer` provides file-level review
  - `sql_generator` turns natural language into SQL
- **Comedy + vibes** — `vibe_oracle.py`, `ComedyArena/`, `DadJokes/`, `KnockKnock/`, `emoji-translator/`, and `sharkbait/` keep the swarm entertaining.

## Project Structure

- `agent.py`, `tools.py` — Ollama CLI agent and tool registry
- `main.py`, `agents/` — Azure-routed utilities (router, repo copilot, commit whisperer, chaos visualizer, code reviewer, SQL generator)
- `config.py` — Azure OpenAI client setup via `DefaultAzureCredential`
- `vibe_oracle.py`, `swarm_chaos.py`, `swarm_mascot.py` — vibe/mascot experiences
- `docs/` — plans and research; `Backlog.md` and `AGENTS.md` document workflow
- `src/` — TypeScript agent prototypes; assorted joke bots live in `ComedyArena/`, `DadJokes/`, `KnockKnock/`, `emoji-translator/`, and `sharkbait/`

## Recent Changes

See [CHANGELOG.md](CHANGELOG.md) for the latest updates.

## Contributing

- Track work with beads (`bd …`) and mirror status in [Backlog.md](Backlog.md); see [AGENTS.md](AGENTS.md) for the required workflow.
- Keep README/structure in sync with new features and update CHANGELOG when shipping meaningful changes.
- Run the relevant entrypoints (`python agent.py` or `python main.py ...`) after edits to ensure nothing regresses.
