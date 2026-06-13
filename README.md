# TokGraph Web3 V3

> **Turn attention into signals. Turn signals into decisions.**

TokGraph is a Web3 narrative intelligence engine that converts TikTok content into structured, actionable crypto market signals.

## Live Demo

Open `index.html` in any browser — no build step required.

GitHub Pages: https://yusufsafary.github.io/tokgraph-web3-v3/

---

## Features

- **Analyze** — Paste any TikTok transcript and extract Web3 narrative intelligence
- **Trend Feed** — Live narrative momentum across crypto attention markets
- **History** — Browse past signal extractions with full details
- **Agent Mode** — REST API for AI agents: `POST /analyze`, `GET /trend`, `GET /history`
- **Offline Demo** — Works without backend using smart mock analysis

## UI Design

- Mobile-first, TikTok-style dark UI
- Neon palette: Cyan `#00F5FF` · Purple `#A855F7` · Green `#00FF85`
- Fonts: Space Grotesk · IBM Plex Mono · Inter
- Animated score bars, sentiment badges, action verdict cards

## API Endpoints

```
POST /analyze     Extract crypto narrative signal from text
GET  /trend       Aggregate narrative momentum data
GET  /history     Past analyses
GET  /health      System status
```

### Example Request

```bash
curl -X POST https://your-backend/analyze \
  -H "Content-Type: application/json" \
  -d '{"text": "AI agents are taking over crypto right now..."}'
```

### Example Response

```json
{
  "id": "abc123",
  "narrative_category": "AI",
  "key_narrative": "AI agent infrastructure emerging",
  "sentiment": "Bullish",
  "market_relevance_score": 8.5,
  "tokens_mentioned": ["NEAR", "FET", "VIRTUAL"],
  "keywords": ["autonomous", "agents", "protocol"],
  "why_it_matters": "AI agent narratives driving significant attention...",
  "action": "Early Signal",
  "timestamp": "2026-06-13T00:00:00.000Z"
}
```

## Tech Stack

- **Frontend**: Single HTML file, vanilla JS, no framework
- **Backend**: Node.js + Express (connect your own)
- **AI**: OpenAI API compatible
- **Storage**: JSON / SQLite (MVP level)

---

*TokGraph Web3 V3 · 2026*
