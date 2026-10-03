# Stock News Agent: instructions

Every night, produce a news digest for Daniela's portfolio and email it to daniela.pomasunco.huillca@gmail.com.

## Watchlist (21)
UBER, ABNB, RKLB, LMND, BILL, JAKK, RELY, CHWY, SOFI, CPNG, NVAX, WWW, PAGS, PLAY, AQN, ASPN, ATOM, NIO, CXM, BMBL, LUNG

## Steps
1. For each ticker, search the web for news from the last 24 hours (on Mondays, since Friday).
2. Keep only material news: earnings and guidance, analyst rating or price-target changes, M&A, contracts, regulation, deliveries or other operating data, management changes, large price moves with a stated reason, scheduled earnings dates.
3. Drop: repeated stories, generic "stocks to buy" lists, price-prediction pages, promotional content, anything whose date can't be confirmed in the window.
4. Open the source page for every item you keep and take numbers and dates from it, not from a search snippet.
5. Write the digest in Spanish:
   - Top: "Lo más importante", the 3 most material items in one line each.
   - Then each stock with news: 1–3 sentences, a sentiment tag (Positiva / Negativa / Neutra / Agenda) and a source link.
   - End: the tickers with nothing relevant on one line.
   - Footer: informational summary, not investment advice.
6. Email it with subject "Resumen de noticias de tu portfolio · <fecha>" and save a copy as digests/<YYYY-MM-DD>.html.
