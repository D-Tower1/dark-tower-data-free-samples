# Sources and citations

All numbers in this repository come from public sources. Each source asks to be credited as shown. The Federal Reserve, FRED, the CFTC and the other sources do not endorse this repository.

## cot

```
SOURCES AND CITATIONS - COT Pack (daily pack)
Data retrieved 2026-11-02 UTC.

U.S. Commodity Futures Trading Commission (CFTC), Commitments of Traders, Futures Only reports, from the CFTC Public
Reporting Environment, https://publicreporting.cftc.gov :
  Traders in Financial Futures (TFF), dataset gpe5-46if: S&P 500, Nasdaq-100, Dow, Russell 2000, 10-year Treasury, Euro, Yen, Pound.
  Disaggregated, dataset 72hh-3qpy: crude oil WTI, natural gas, gold, silver, copper.

Contract market codes: S&P 500 (E-mini) 13874A; Nasdaq-100 (E-mini) 209742; Dow Jones (DJIA x $5) 124603; Russell 2000 (E-mini) 239742/23977A; Crude oil WTI 067651; Natural gas (Henry Hub) 023651; Gold 088691; Silver 084691; Copper 085692; 10-year US Treasury note 043602; Euro FX 099741; Japanese yen 097741; British pound 096742.
Russell 2000: reports before August 2017 come from the ICE Futures U.S. contract (23977A), later ones from the CME contract (239742).

The CFTC dataset metadata names no required citation wording or licence; we credit the CFTC as the source.
Net position = long minus short, per trader type. The week-over-week change is our calculation: this report's net minus the
net of the previous published report (holiday weeks shift the date). Positions are numbers of futures contracts.

This product is not endorsed by the CFTC.
```

## gold_drivers

```
SOURCES AND CITATIONS - Gold Drivers (daily pack)
Data retrieved 2026-11-03 UTC.

FRED series. Each source asks to be cited as follows (FRED's "Suggested Citation"):

[DFF] Board of Governors of the Federal Reserve System (US), Federal Funds Effective Rate [DFF], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DFF, .

[CPIAUCSL] U.S. Bureau of Labor Statistics, Consumer Price Index for All Urban Consumers: All Items in U.S. City Average [CPIAUCSL], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/CPIAUCSL, .

[PCEPI] U.S. Bureau of Economic Analysis, Personal Consumption Expenditures: Chain-type Price Index [PCEPI], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/PCEPI, .

[UNRATE] U.S. Bureau of Labor Statistics, Unemployment Rate [UNRATE], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/UNRATE, .

[ICSA] U.S. Employment and Training Administration, Initial Claims [ICSA], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/ICSA, .

[DFII10] Board of Governors of the Federal Reserve System (US), Market Yield on U.S. Treasury Securities at 10-Year Constant Maturity, Quoted on an Investment Basis, Inflation-Indexed [DFII10], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DFII10, .

[DTWEXBGS] Board of Governors of the Federal Reserve System (US), Nominal Broad U.S. Dollar Index [DTWEXBGS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DTWEXBGS, .

[DGS10] Board of Governors of the Federal Reserve System (US), Market Yield on U.S. Treasury Securities at 10-Year Constant Maturity, Quoted on an Investment Basis [DGS10], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DGS10, .

Derived series BREAKEVEN_10Y: calculated by Tower from two of the series above:
  10-year breakeven inflation = DGS10 minus DFII10 (same day, percentage points).
  It is our own calculation, not a number published by FRED or the Federal Reserve.

Commitments of Traders (COT):
U.S. Commodity Futures Trading Commission, Commitments of Traders, Disaggregated Futures Only report,
GOLD - COMMODITY EXCHANGE INC. (contract market code 088691), https://publicreporting.cftc.gov (dataset 72hh-3qpy).
The CFTC dataset metadata names no required citation wording or licence; we credit the CFTC as the source.
Net managed-money position = managed-money long minus managed-money short; the week-over-week change is our calculation.
COT_GOLD_HISTORY.csv is built from the CFTC historical compressed files (fut_disagg_txt_YYYY.zip, https://www.cftc.gov/MarketReports/CommitmentsofTraders/HistoricalCompressed/index.htm). The change is versus the previous published report (holiday weeks shift the date).

FRED is a service of the Federal Reserve Bank of St. Louis. This product is not endorsed by FRED, the Federal Reserve,
the BLS, the BEA, the Employment and Training Administration or the CFTC.
```

## fed_forex

```
SOURCES AND CITATIONS - Forex Daily (Federal Reserve rates), daily pack
Data retrieved 2026-11-03 UTC.

All numbers come from the Federal Reserve Board's H.10 'Foreign Exchange Rates' release, as distributed by FRED, and the
Board's broad dollar index. FRED marks every series below 'Public Domain: Citation Requested'. FRED asks to be cited like this
(FRED's "Suggested Citation"):

[DEXUSEU] Board of Governors of the Federal Reserve System (US), U.S. Dollars to Euro Spot Exchange Rate [DEXUSEU], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXUSEU, .

[DEXUSUK] Board of Governors of the Federal Reserve System (US), U.S. Dollars to U.K. Pound Sterling Spot Exchange Rate [DEXUSUK], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXUSUK, .

[DEXUSAL] Board of Governors of the Federal Reserve System (US), U.S. Dollars to Australian Dollar Spot Exchange Rate [DEXUSAL], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXUSAL, .

[DEXUSNZ] Board of Governors of the Federal Reserve System (US), U.S. Dollars to New Zealand Dollar Spot Exchange Rate [DEXUSNZ], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXUSNZ, .

[DEXJPUS] Board of Governors of the Federal Reserve System (US), Japanese Yen to U.S. Dollar Spot Exchange Rate [DEXJPUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXJPUS, .

[DEXCAUS] Board of Governors of the Federal Reserve System (US), Canadian Dollars to U.S. Dollar Spot Exchange Rate [DEXCAUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXCAUS, .

[DEXSZUS] Board of Governors of the Federal Reserve System (US), Swiss Francs to U.S. Dollar Spot Exchange Rate [DEXSZUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXSZUS, .

[DEXCHUS] Board of Governors of the Federal Reserve System (US), Chinese Yuan Renminbi to U.S. Dollar Spot Exchange Rate [DEXCHUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXCHUS, .

[DEXKOUS] Board of Governors of the Federal Reserve System (US), South Korean Won to U.S. Dollar Spot Exchange Rate [DEXKOUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXKOUS, .

[DEXINUS] Board of Governors of the Federal Reserve System (US), Indian Rupees to U.S. Dollar Spot Exchange Rate [DEXINUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXINUS, .

[DEXMXUS] Board of Governors of the Federal Reserve System (US), Mexican Pesos to U.S. Dollar Spot Exchange Rate [DEXMXUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXMXUS, .

[DEXBZUS] Board of Governors of the Federal Reserve System (US), Brazilian Reals to U.S. Dollar Spot Exchange Rate [DEXBZUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXBZUS, .

[DEXSDUS] Board of Governors of the Federal Reserve System (US), Swedish Kronor to U.S. Dollar Spot Exchange Rate [DEXSDUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXSDUS, .

[DEXSFUS] Board of Governors of the Federal Reserve System (US), South African Rand to U.S. Dollar Spot Exchange Rate [DEXSFUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXSFUS, .

[DEXTAUS] Board of Governors of the Federal Reserve System (US), Taiwan Dollars to U.S. Dollar Spot Exchange Rate [DEXTAUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXTAUS, .

[DEXHKUS] Board of Governors of the Federal Reserve System (US), Hong Kong Dollars to U.S. Dollar Spot Exchange Rate [DEXHKUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXHKUS, .

[DEXSIUS] Board of Governors of the Federal Reserve System (US), Singapore Dollars to U.S. Dollar Spot Exchange Rate [DEXSIUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXSIUS, .

[DEXNOUS] Board of Governors of the Federal Reserve System (US), Norwegian Kroner to U.S. Dollar Spot Exchange Rate [DEXNOUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXNOUS, .

[DEXDNUS] Board of Governors of the Federal Reserve System (US), Danish Kroner to U.S. Dollar Spot Exchange Rate [DEXDNUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXDNUS, .

[DEXTHUS] Board of Governors of the Federal Reserve System (US), Thai Baht to U.S. Dollar Spot Exchange Rate [DEXTHUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXTHUS, .

[DEXMAUS] Board of Governors of the Federal Reserve System (US), Malaysian Ringgit to U.S. Dollar Spot Exchange Rate [DEXMAUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXMAUS, .

[DEXSLUS] Board of Governors of the Federal Reserve System (US), Sri Lankan Rupees to U.S. Dollar Spot Exchange Rate [DEXSLUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DEXSLUS, .

[DTWEXBGS] Board of Governors of the Federal Reserve System (US), Nominal Broad U.S. Dollar Index [DTWEXBGS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DTWEXBGS, .

What the H.10 rates are: noon buying rates in New York City for cable transfers payable in foreign currencies, one
value per business day. They are published by the Federal Reserve, normally once a week (Monday, for the week before).
Pair names: EUR_USD, GBP_USD, AUD_USD and NZD_USD are US dollars per one euro / pound / Australian dollar / New Zealand
dollar. Every other pair USD_xxx is units of that currency per one US dollar. Values are exactly as published; we do not
invert, smooth, fill or round them.

FRED is a service of the Federal Reserve Bank of St. Louis. This product is not endorsed by FRED or the Federal Reserve.
```
