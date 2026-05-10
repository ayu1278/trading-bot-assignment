
# Binance Futures Testnet Trading Bot

## Features
- Place MARKET and LIMIT orders
- BUY and SELL support
- CLI based input
- Logging support
- Error handling and validation
- Structured reusable code

---

## Setup

### 1. Clone project
```bash
git clone <your-repo>
cd trading_bot
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Create `.env`
```env
API_KEY=your_api_key
API_SECRET=your_api_secret
```

### 4. Run Project

### MARKET Order
```bash
python cli.py --symbol BTCUSDT --side BUY --type MARKET --quantity 0.001
```

### LIMIT Order
```bash
python cli.py --symbol BTCUSDT --side SELL --type LIMIT --quantity 0.001 --price 70000
```

---

## Project Structure

```text
trading_bot/
│
├── bot/
│   ├── __init__.py
│   ├── client.py
│   ├── orders.py
│   ├── validators.py
│   └── logging_config.py
│
├── logs/
├── cli.py
├── requirements.txt
└── README.md
```

---

## Assumptions
- Binance Futures USDT-M Testnet used
- User already has API keys
- LIMIT orders use GTC timeInForce

