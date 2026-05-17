# APEX Ticker Research — Chris Drop Zone

## How This Works
1. Copy/paste your Gemini research into the `incoming/` folder
2. Name files: `YYYY-MM-DD_batch-N_ticker-start_ticker-end.md`
   - Example: `2026-05-17_batch-01_NVDA_KO.md`
3. Atlas will auto-ingest, parse, and store into:
   - **PostgreSQL**: `stock_fundamentals`, `tracked_stocks`
   - **Neo4j**: Supply chain nodes, competitor edges, dependency graphs
   - **Vector/RAG**: Full research corpus for retrieval

## Research Template (10 Sections per Ticker)
1. Business Identity (what they do, #1 revenue driver, moat)
2. Supply Chain Dependencies (top 3 suppliers, raw materials, single-source risk, geo concentration)
3. Customer Base (top 3 segments, consumer/enterprise/govt split, geo revenue, concentration risk)
4. Competitive Landscape (top 3 competitors + market share, disruption risk, regulatory risk)
5. Financial Snapshot (market cap, P/E, Fwd P/E, PEG, P/S, P/B, revenue TTM, YoY growth, margins, FCF, debt/equity, dividend)
6. Growth Catalysts (3 drivers next 12mo, 3 drivers next 5yr, pipeline events)
7. Risk Factors (3 existential, 3 near-term headwinds, geopolitical exposure)
8. Price Targets (current price, Wall St consensus 12mo, YOUR predictions: 1mo/6mo/12mo/5yr/10yr with confidence 1-10)
9. Sentiment Signals (institutional trend, insider activity, short interest, analyst momentum)
10. Big Picture (ONE thing to know, what reverses your thesis)

## Formatting
- Use `## TICKER: COMPANY NAME` as the header for each stock
- Keep each section as `### Section N: Name`
- Separate tickers with `---`

## Don't overthink the format — Atlas will parse it all.
