# Environment

## Platform
- **OS:** Windows 11
- **Shell:** PowerShell 7+ (pwsh)
- **Terminal:** Windows Terminal

## Docker
- **Docker Desktop:** Running
- **Hermes container:** Running (port 9119)
- **Container image:** hermes-agent 0.17.0
- **Named volume:** `hermes-data` → `/home/hermes/.hermes`
- **Bind mount:** `./my-project:/workspace:rw`

## Local LLM
- **Endpoint:** `http://host.docker.internal:8033/v1`
- **Protocol:** OpenAI-compatible chat completions API

## Hermes Configuration
- **Config file:** `~/.hermes/config.yaml`
- **Env file:** `~/.hermes/.env`
- **Log files:** `~/.hermes/logs/agent.log`, `~/.hermes/logs/errors.log`
- **Cron jobs:** `~/.hermes/cron/jobs.json`

## Vault Configuration
- **Vault path:** `C:\Users\ap-mining\VisualCode\Obsidian\ME`
- **Vault git:** Initialized, remote `https://github.com/JTYEG/obsidian`
- **Vault .gitignore:** Present and configured
- **OBSIDIAN_VAULT_PATH:** Not yet set in `.env`

## Network
- **Dashboard:** http://localhost:9119
- **LLM:** http://host.docker.internal:8033/v1

## Dependencies
- Python 3.11-slim (Docker base image)
- hermes-agent 0.17.0
- croniter (cron expression parsing)
- No external package dependencies beyond hermes-agent
