# Make Skill

[![Author](https://img.shields.io/badge/Author-Daniel_Rudaev-000000?style=flat)](https://github.com/daniel-rudaev)
[![Studio](https://img.shields.io/badge/Studio-D1DX-000000?style=flat)](https://d1dx.com)
[![Make](https://img.shields.io/badge/Make-Skill-6D00CC?style=flat&logo=make&logoColor=white)](https://make.com)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat)](./LICENSE)

A complete reference for the Make.com API and blueprint management — covering scenario CRUD, blueprint JSON structure, expression syntax, router filters, error handlers, connections, webhooks, data stores, execution history, and Make-to-n8n migration mapping. Built from real production work at [D1DX](https://d1dx.com).

## What's Included

| Topic | What it covers |
|-------|---------------|
| API Basics | Base URL, auth, pagination, team ID requirement, MCP usage |
| Scenarios | List, get, activate/deactivate, create, delete |
| Blueprints | Get and push blueprints, full JSON structure, key module names reference |
| Expression Syntax | `{{1.body}}` references, `ifempty`, `lower`, `formatDate`, `parseDate`, `toNumber`, `length` |
| Router Filters | Condition structure, AND/OR logic, full operator reference |
| Error Handlers | `Ignore`, `Resume`, `Rollback`, `Break`, `Commit` handler types |
| Connections | List, get, test connection health |
| Webhooks (Hooks) | List, get, create, delete; production URL retrieval |
| Data Stores | List stores, read/write records |
| Execution History | List scenario execution logs, status values |
| Make-to-n8n Migration | Module mapping table, expression syntax translation table |
| Critical Gotchas | Blueprint-as-string encoding, zone prefix requirement, connection ID portability, pull-before-edit, activation after push |

## Install

### Claude Code

```bash
git clone https://github.com/D1DX/make-skill.git
cp -r make-skill ~/.claude/skills/make
```

Or as a git submodule:

```bash
git submodule add https://github.com/D1DX/make-skill.git path/to/skills/make
```

### Other AI Agents

Copy `SKILL.md` (and supporting files) into your agent's prompt or knowledge directory. The skill is structured markdown — works with any LLM agent that reads reference files.

## Structure

```
make-skill/
├── SKILL.md    — Main skill file
└── README.md   — This file
```

## Sources

Distilled from managing 257 Make.com scenarios at D1DX and executing a large-scale migration to n8n. Covers API patterns, blueprint engineering, and migration mappings developed through hands-on scenario auditing, blueprint editing, and cross-platform porting.

## Credits

Built by [Daniel Rudaev](https://github.com/daniel-rudaev) at [D1DX](https://d1dx.com).

## License

MIT License — Copyright (c) 2026 Daniel Rudaev @ D1DX
