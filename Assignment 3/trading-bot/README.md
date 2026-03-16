# Binance Futures Testnet Trading Bot

A simple Python CLI application to place MARKET and LIMIT orders on Binance Futures Testnet.

---

## Features

- Place MARKET orders
- Place LIMIT orders
- Supports BUY and SELL
- CLI input validation
- Structured project architecture
- Logging of requests and errors
- Exception handling

---

## Setup

### 1 Install Python

Python 3.8+

---

### 2 Clone Repository

git clone https://github.com/yourusername/trading-bot
cd trading-bot

---

### 3 Install Dependencies

pip install -r requirements.txt

---

### 4 Create Environment File

Create `.env`


BINANCE_API_KEY=your_api_key
BINANCE_API_SECRET=your_secret


---

### 5 Binance Testnet

Register here:

https://testnet.binancefuture.com

Generate API Keys.

---

# Running the Bot

## MARKET ORDER
python cli.py --symbol BTCUSDT --side BUY --type MARKET --quantity 0.001


## LIMIT ORDER
python cli.py --symbol BTCUSDT --side SELL --type LIMIT --quantity 0.001 --price 60000



# Example Output


Order Request Summary
Symbol: BTCUSDT
Side: BUY
Type: MARKET
Quantity: 0.001

Order placed successfully!

Order Details
Order ID: 12345678
Status: FILLED
Executed Qty: 0.001
Avg Price: 59120



Logs include

- API request details
- API responses
- errors

---

# Assumptions

- Only USDT-M Futures
- Price required only for LIMIT orders
- User provides valid symbol supported by Binance

---

# Author

Rahul Kumar Chaudhary