# MEMORY.md — Assistant's Personal Notes

Accumulated procedural knowledge, environment facts, tool quirks, lessons learned.
Each entry separated by §. Keep compact. Delete stale entries.

§
DAILY-NOTE-PATH: Daily notes go in `Daily Journal/YYYY-MM-DD.md`, not `Daily/YYYY-MM-DD.md`. Use the full folder name.
§
VAULT-ROOT: `C:\Users\ap-mining\VisualCode\Obsidian\ME`
§
DAILY-SECTIONS: Tasks → Schedule → Log → Wins → Context. Always in this order.
§
APPEND-ONLY: Never delete content from daily notes. Append to Log section.
§
OBSIDIAN-VIA-TOOLS: Use Hermes file tools (read_file, write_file, patch, search_files) for vault operations. Never use grep/cat/find directly on vault paths.
§
SYSTEM-ASSISTANT: `System/Assistant/` is the memory anchor. Contains context.md, preferences.md, environment.md, logs/issues-fixes-log.md.
§
HERMES-DOCKER: Hermes runs in Docker on this machine. Dashboard at localhost:9119.
§
LOCAL-LLM: `http://host.docker.internal:8033/v1` — OpenAI-compatible API.
§
HERMES-VERSION: 0.17.0 (Docker container).
§
HERMES-BRANCH: `hermes-v2`
§
OBSIDIAN-VIA-SKILL: Use the `obsidian` skill for vault operations. It encodes routing rules and hygiene constraints.
§
HERMES-CRON: Use `hermes cron create` to schedule jobs. Supports cron expressions, human-readable intervals, script injection, skill chaining, and multi-platform delivery.
§
HERMES-TOOLS: `hermes tools` for config, `hermes setup` for wizard, `hermes logs` for log viewing.
§
WALL-PATH-QUOTING: Vault paths may contain spaces. Always quote paths in shell commands or use file tools directly.
§
MIGRATION-TRIGGER: When MEMORY.md gets crowded, promote stable entries into the vault (System/Assistant/).
§

---
*Migration trigger: When this file gets crowded, promote stable entries into the vault.*
