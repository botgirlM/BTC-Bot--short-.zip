# btc-short-bot

Small demo crypto trading bot that attempts to profit from BTC declines using an EMA crossover shorting strategy.

Features
- Paper-trading by default
- Optional live futures path using `ccxt` (exchange-specific)
- Small Flask dashboard to view price, EMAs, signals, position and simulated P&L

Setup
1. Create a virtualenv and install:
   ```
   python -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```
2. Copy `config.example.json` to `config.json` and edit values. Keep `paper: true` while testing.
3. Run:
   ```
   python app.py
   ```
4. Open http://localhost:8080

Important
- Do not commit real API keys
- This code is educational only. Use extreme caution before enabling live trading
