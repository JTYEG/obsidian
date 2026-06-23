# Context

## Hermes Operational Context

Hermes is a personal AI agent running in a Docker container on this machine.
It connects to a local LLM served at `http://host.docker.internal:8033/v1`.

### Deployment
- **Platform:** Windows 11
- **Runtime:** Docker Desktop
- **Hermes version:** 0.17.0
- **Dashboard:** http://localhost:9119
- **Local LLM:** `http://host.docker.internal:8033/v1`

### Workspace
- **Hermes code repo:** `C:\Users\ap-mining\VisualCode\Hermes` (branch: `hermes-v2`)
- **Obsidian vault:** `C:\Users\ap-mining\VisualCode\Obsidian\ME`
- **Vault git remote:** `https://github.com/JTYEG/obsidian`

### Current Projects
- Hermes V2 Obsidian integration — connecting Hermes to the Obsidian vault as persistent memory
- Docker deployment of Hermes — running in a container with local LLM endpoint

### Known Quirks and Constraints
- WSL/bash has issues writing files outside the Docker context — use PowerShell or write from inside the container
- The vault should never be merged into the Hermes repo — they are separate repos with different lifecycles
- `.obsidian/` and `.smart-env/` are application state — never write generated content there
- Prompt caching is critical — avoid mutating past conversation context mid-session
- Hermes uses `OBSIDIAN_VAULT_PATH` env var to locate the vault — must be set in `.env`
