# Hermes Dashboard

Real-time monitoring dashboard for Hermes AI agent system.

## Features

- **Live WebSocket updates** — real-time KPIs every 3 seconds
- **Agent tree** — visualize active sessions, tasks, and sub-agents
- **System metrics** — CPU load, memory usage, uptime
- **Gateway status** — connected platforms and active agents
- **Socat monitoring** — port forwarding health checks
- **PWA support** — installable on mobile/desktop
- **iOS Widget** — Scriptable widget for quick status glance

## Tech Stack

- **Backend:** Python / FastAPI + WebSocket
- **Frontend:** Vanilla JS + CSS (no frameworks)
- **Data:** SQLite (Hermes state.db + kanban.db)

## Quick Start

```bash
pip install -r requirements.txt
python server.py
```

Open http://localhost:3333

## API

- `GET /api/snapshot` — Full dashboard state (JSON)
- `WS /ws` — Real-time push (send "ping" for keepalive)

## Links

- Live: https://status.proyectos.cristiancode.dev
- Repo: https://github.com/cristiancode-hermes/hermes-dashboard
