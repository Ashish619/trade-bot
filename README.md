# trade-bot

An AI-enabled trading platform built as a Node.js web app, using [Kite Connect](https://kite.trade/docs/connect/v3/) (Zerodha) for market data and order execution.

> **Disclaimer:** Educational project. Trading involves substantial risk of loss. Paper trade first and never risk money you can't afford to lose.

## Vision

- Live and historical market data from Kite Connect (REST + WebSocket ticker)
- AI-assisted analysis and signal generation
- Strategy engine with backtesting and paper trading
- Risk management (position sizing, stop-loss, max drawdown)
- Web dashboard for watchlists, positions, orders and P&L

## Tech Stack (planned)

- Node.js (backend API, Kite Connect integration via `kiteconnect`)
- Web frontend (React / Next.js)
- AI layer for analysis and signals
- SQLite/Postgres for storing candles, trades and logs

## Getting Started

```bash
git clone https://github.com/Ashish619/trade-bot.git
cd trade-bot
npm install
cp .env.example .env   # add KITE_API_KEY and KITE_API_SECRET
npm run dev
```

Kite Connect access tokens expire daily, so the app needs a login flow that exchanges the `request_token` for a fresh `access_token` each trading day.

## Configuration

Secrets live in `.env` (git-ignored). Never commit API keys or access tokens.

## Roadmap

- [ ] Project skeleton (Node.js + web UI)
- [ ] Kite Connect login and token handling
- [ ] Market data: quotes, historical candles, WebSocket ticks
- [ ] Strategy interface and backtester
- [ ] AI analysis/signal module
- [ ] Paper trading
- [ ] Live order placement with risk limits
- [ ] Dashboard

## License

TBD
