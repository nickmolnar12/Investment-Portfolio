# Portfolio Dashboard

A single-page financial dashboard that displays a live view of my stock portfolio.
It fetches real-time price quotes from the Finnhub API and renders them across four panels:
a donut chart showing allocation by position (including cash), a holdings list with per-share
cost basis and unrealized gain/loss, a sector breakdown with proportional bar charts, and an
account summary grid showing total earnings, unrealized P&L, and daily change. An Advisor
Insight section at the bottom provides a static narrative analysis of the portfolio's
composition and risk profile.

---

## Updating The Data

All personal portfolio data is located in the script section at the bottom of index.html.

- Stocks/positions: find the `stocks` array (line 163). Each entry contains the ticker,
  display name, number of shares, average cost basis per share, and sector.

- Cash balance: `const CASH_VAL` (line 155)

- Net deposits: `const NET_DEPOSITS` (line 156)

- Realized earnings: `const REALIZED` (line 157)

- Hardcoded breakdown figures (stats grid): lines 222-223

- To swap data providers: update `API_KEY` (line 154) and the Finnhub fetch URL (line 176)
