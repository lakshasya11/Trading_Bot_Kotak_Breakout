# 🤖 Trading Bot — Kotak Breakout Strategy

An algorithmic trading bot with a **FastAPI backend** and **React frontend dashboard**, built for real-time options trading using the Kotak Neo API.

---

## 📁 Project Structure

```
Trading_Bot_Kotak_Breakout/
├── backend/        # FastAPI server, broker integration, strategy engine
├── frontend/       # React dashboard (Vite + MUI)
├── START_EVERYTHING.bat
└── STOP_EVERYTHING.bat
```

---

## ✨ Features

- 🔐 Auto-login with Kotak Neo broker API
- 📡 Real-time market data via WebSockets
- 📊 Multi-strategy engine (RSI, MA Crossover, Candlestick Patterns, UOA Scanner)
- 🛡️ Risk management & trailing stop-loss
- 📈 Live React dashboard with candlestick charts, option chain, P&L tracking
- 🔔 Audio & visual trade alerts
- 🗃️ SQLite trade logging & analytics

---

## 🛠️ Tech Stack

| Layer    | Tech                                      |
|----------|-------------------------------------------|
| Backend  | Python, FastAPI, Uvicorn, KiteConnect     |
| Frontend | React 18, Vite, Material-UI, TradingView  |
| Database | SQLite                                    |
| Broker   | Kotak Neo API                             |

---

## ⚙️ Setup

### Backend

```bash
cd backend
python -m venv venv
venv\Scripts\activate        # Windows
pip install -r requirements.txt
```

Create a `.env` file in `backend/`:
```env
API_KEY=your_kotak_api_key
API_SECRET=your_kotak_api_secret
```

Run:
```bash
uvicorn main:app --reload --port 8000
```

### Frontend

```bash
cd frontend
npm install
npm run dev
```

---

## 🚀 Quick Start (Windows)

Just double-click:
```
START_EVERYTHING.bat   ← starts backend + frontend
STOP_EVERYTHING.bat    ← stops everything
```

---

## ⚠️ Important

- Never commit `.env`, `broker_config.json`, `strategy_params.json`, or `*.db` files
- All sensitive files are listed in `.gitignore`

---

## 📄 License

For personal/educational use only. Not financial advice.
