# Stock News Agent

An AI agent that reads the news on my 21 stock holdings every evening, keeps only what matters and emails me a short digest.

**[See a real digest (3 Oct 2026)](digests/2026-10-03.html)** · **[Agent instructions](prompt.md)**

## The problem

Following news for 21 stocks by hand is slow, and most headlines are noise: repeated stories, "stocks to buy" lists and price predictions.

## How it works

1. A scheduled Claude routine runs every evening at around 6pm London time.
2. For each stock it searches the last 24 hours of news.
3. It keeps only material events: earnings and guidance, analyst rating changes, contracts, M&A, regulation, operating data and scheduled earnings dates.
4. It opens the source page for every item it keeps and takes numbers and dates from there, not from a search snippet.
5. It emails me the digest: the 3 most important items on top, then each stock with a sentiment tag (positive, negative, neutral, calendar) and a source link, then the stocks with nothing relevant.

## First run

On 3 Oct 2026 it checked 21 stocks, reported 8 with material news and set aside 13 with nothing relevant.

## Watchlist

UBER, ABNB, RKLB, LMND, BILL, JAKK, RELY, CHWY, SOFI, CPNG, NVAX, WWW, PAGS, PLAY, AQN, ASPN, ATOM, NIO, CXM, BMBL, LUNG

## Built with

Claude (scheduled routine, web search, Gmail connector). The whole agent is defined in plain language in [prompt.md](prompt.md), so changing what it looks for means editing a text file, not code.

*Informational summary, not investment advice.*
