# Finance

## Project overview
**Finance** is a web application (Flask) that lets users simulate buying and selling stocks. Users register and log in, look up real-time stock quotes, buy and sell shares, view their portfolio with current prices and values, and review transaction history. The app uses a SQL database (SQLite) for persistence and a stock price lookup API for current prices.

This README describes how to run the project, the database schema, important files, and notes about implementation.

---

## Features
- Register and login (passwords hashed).
- Look up current stock quotes (by ticker symbol).
- Buy shares (requires sufficient cash).
- Sell shares (only if user owns enough shares).
- Portfolio overview showing current holding values and remaining cash.
- Transaction history listing buys and sells with timestamps and prices.
- Input validation and helpful error messages.

---

## Requirements
- Python 3.8+ (compatible with 3.9/3.10)
- Flask
- CS50 library (optional but commonly used in CS50 solutions)
- SQLite (comes standard with Python)
- `requests` (for API calls)
- `werkzeug` (password hashing functions; available via Flask)
- Environment to run: local machine or supported cloud environment

Install dependencies (example):

```bash
python -m venv venv
source venv/bin/activate        # macOS / Linux
# venv\Scripts\activate         # Windows (PowerShell)
pip install flask cs50 requests

