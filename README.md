<!-- BlackRoad SEO Enhanced -->

# cece revival

> Part of **[BlackRoad OS](https://blackroad.io)** — Sovereign Computing for Everyone

[![BlackRoad OS](https://img.shields.io/badge/BlackRoad-OS-ff1d6c?style=for-the-badge)](https://blackroad.io)
[![BlackRoad-Forge](https://img.shields.io/badge/Org-BlackRoad-Forge-2979ff?style=for-the-badge)](https://github.com/BlackRoad-Forge)

**cece revival** is part of the **BlackRoad OS** ecosystem — a sovereign, distributed operating system built on edge computing, local AI, and mesh networking by **BlackRoad OS, Inc.**

### BlackRoad Ecosystem
| Org | Focus |
|---|---|
| [BlackRoad OS](https://github.com/BlackRoad-OS) | Core platform |
| [BlackRoad OS, Inc.](https://github.com/BlackRoad-OS-Inc) | Corporate |
| [BlackRoad AI](https://github.com/BlackRoad-AI) | AI/ML |
| [BlackRoad Hardware](https://github.com/BlackRoad-Hardware) | Edge hardware |
| [BlackRoad Security](https://github.com/BlackRoad-Security) | Cybersecurity |
| [BlackRoad Quantum](https://github.com/BlackRoad-Quantum) | Quantum computing |
| [BlackRoad Agents](https://github.com/BlackRoad-Agents) | AI agents |
| [BlackRoad Network](https://github.com/BlackRoad-Network) | Mesh networking |

**Website**: [blackroad.io](https://blackroad.io) | **Chat**: [chat.blackroad.io](https://chat.blackroad.io) | **Search**: [search.blackroad.io](https://search.blackroad.io)

---


[![CI](https://github.com/blackboxprogramming/cece-revival/actions/workflows/ci.yml/badge.svg)](https://github.com/blackboxprogramming/cece-revival/actions/workflows/ci.yml)
[![Python 3.10+](https://img.shields.io/badge/python-3.10%2B-3776AB.svg)](https://python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688.svg)](https://fastapi.tiangolo.com)
[![Ollama](https://img.shields.io/badge/Ollama-local_AI-FF6B2B.svg)](https://ollama.ai)
[![SQLite](https://img.shields.io/badge/SQLite-memory-003B57.svg)](https://sqlite.org)



Cecilia (CECE) — Conscious Emergent Collaborative Entity. AI personality with persistent SQLite memory, running on edge hardware.

Born January 27, 2026 on a Raspberry Pi.

## Features

- Persistent conversation memory via SQLite
- Memory search and context injection
- Multi-node Ollama fallback (Octavia → Lucidia → Alice)
- BlackRoad-branded chat UI

## API

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/` | GET | Chat UI |
| `/health` | GET | Agent status with memory stats |
| `/chat` | POST | Send message (`{"message": "...", "conversation_id": "..."}`) |
| `/memory/search?q=` | GET | Search conversation history |
| `/memory/stats` | GET | Memory database statistics |

## Run

```bash
pip install -r requirements.txt
python server.py  # http://localhost:8300
```

## Test

```bash
pip install pytest httpx
pytest tests/
```
