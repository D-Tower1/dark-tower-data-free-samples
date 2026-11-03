# Dark Tower Data - free samples (COT, Gold Drivers, Federal Reserve forex rates)
    
    A small, free slice of three datasets from [Dark Tower Data](https://darktowerdata.com): the **last 12 weeks** of each, as plain CSV files, so you can try the formats in a notebook before using the full data.
    Everything comes from **public sources** (US government data: the CFTC, the Federal Reserve Board via FRED, the BLS and BEA). It is information, not investment advice.
    
    ## What is in `data/`
    
    | folder | what it is |
    |---|---|
    | `cot/` | CFTC Commitments of Traders, 13 markets (S&P 500, Nasdaq-100, Dow, Russell 2000, crude oil, natural gas, gold, silver, copper, 10-year Treasury note, euro, yen, pound): the last 12 weekly reports per market, by type of trader, plus `COT_LATEST.csv` (newest report, all markets) |
    | `gold_drivers/` | What gold is watched next to: Fed funds rate, 10-year real yield, 10-year breakeven inflation (our calculation), broad dollar index (last 12 weeks); CPI, PCE prices and unemployment (last 3 months); jobless claims (last 12 weeks); CFTC gold positioning (last 12 weekly reports). No gold price. |
    | `fed_forex/` | The Federal Reserve's H.10 daily exchange rates of the US dollar against 22 currencies (last 12 weeks) and the latest rate and change per pair. One noon rate per business day; **not live prices**. |
    
    Built from our daily packs dated: COT 2026-11-02, Gold Drivers 2026-11-03, Forex Daily (Federal Reserve rates) 2026-11-03.
    
    Files (rows, first and last date):
    ```
      data/cot/COT_LATEST.csv  (65 rows, 2026-10-27 to 2026-10-27)
  data/cot/british_pound.csv  (12 rows, 2026-08-11 to 2026-10-27)
  data/cot/copper.csv  (12 rows, 2026-08-11 to 2026-10-27)
  data/cot/crude_oil_wti.csv  (12 rows, 2026-08-11 to 2026-10-27)
  data/cot/dow.csv  (12 rows, 2026-08-11 to 2026-10-27)
  data/cot/euro_fx.csv  (12 rows, 2026-08-11 to 2026-10-27)
  data/cot/gold.csv  (12 rows, 2026-08-11 to 2026-10-27)
  data/cot/japanese_yen.csv  (12 rows, 2026-08-11 to 2026-10-27)
  data/cot/nasdaq.csv  (12 rows, 2026-08-11 to 2026-10-27)
  data/cot/natural_gas.csv  (12 rows, 2026-08-11 to 2026-10-27)
  data/cot/russell2000.csv  (12 rows, 2026-08-11 to 2026-10-27)
  data/cot/silver.csv  (12 rows, 2026-08-11 to 2026-10-27)
  data/cot/sp500.csv  (12 rows, 2026-08-11 to 2026-10-27)
  data/cot/treasury_10y.csv  (12 rows, 2026-08-11 to 2026-10-27)
  data/fed_forex/FED_FX_DAILY.csv  (58 rows, 2026-08-10 to 2026-10-30)
  data/fed_forex/FED_FX_LATEST.csv  (22 rows, latest per pair)
  data/gold_drivers/BREAKEVEN_10Y.csv  (58 rows, 2026-08-10 to 2026-10-30)
  data/gold_drivers/CPIAUCSL.csv  (3 rows, 2026-07-01 to 2026-09-01)
  data/gold_drivers/DFF.csv  (84 rows, 2026-08-08 to 2026-10-30)
  data/gold_drivers/DFII10.csv  (58 rows, 2026-08-10 to 2026-10-30)
  data/gold_drivers/DTWEXBGS.csv  (58 rows, 2026-08-10 to 2026-10-30)
  data/gold_drivers/ICSA.csv  (12 rows, 2026-08-08 to 2026-10-24)
  data/gold_drivers/PCEPI.csv  (3 rows, 2026-07-01 to 2026-09-01)
  data/gold_drivers/UNRATE.csv  (3 rows, 2026-07-01 to 2026-09-01)
  data/gold_drivers/cot_gold_history.csv  (12 rows, 2026-08-11 to 2026-10-27)
  data/gold_drivers/cot_gold_latest.csv  (1 rows, 2026-10-27 to 2026-10-27)
    ```
    
    ## Want more?
    
    - **Full history and daily updates:** the monthly packs (COT Pack, Gold Drivers, Forex Daily from Federal Reserve rates) and the **one-time 10-Year History bundles** are at **https://darktowerdata.com/products/**
    - Each pack comes with a README, the source citations and the terms of use.
    
    ## Sources and licence
    
    - Sources and the citation each one asks for: see `SOURCES.md`.
    - The underlying numbers are US government data. This selection, the file layout and this README are by Dark Tower Data and are shared under **CC BY 4.0** (credit "Dark Tower Data, https://darktowerdata.com"); see `LICENSE.txt`. The licence covers this free slice only, not our paid packs.
    - Data can be revised by the source later. No warranty; use at your own risk. This is not financial advice.
    