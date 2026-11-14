# Sources and citations

All numbers in this repository come from public sources. Each source asks to be credited as shown. The Federal Reserve, the CFTC and the other sources do not endorse this repository.

## cot

```
SOURCES AND CITATIONS - COT Pack (daily pack)
Data retrieved 2026-11-13 UTC.

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
Data retrieved 2026-11-13 UTC.

Every number comes straight from the agency that publishes it. The series names (DFF, DFII10 and so on) are only the
file names we use; they are the same names as in earlier packs.

[DFF] Board of Governors of the Federal Reserve System (US), Federal Reserve Statistical Release H.15, Selected Interest Rates: Federal funds (effective), every calendar day, percent, not seasonally adjusted (DDP series RIFSPFF_N.D), https://www.federalreserve.gov/releases/h15/

[DFII10] Board of Governors of the Federal Reserve System (US), Federal Reserve Statistical Release H.15, Selected Interest Rates: U.S. Treasury inflation-indexed securities, 10-year constant maturity, daily, percent (DDP series RIFLGFCY10_XII_N.B), https://www.federalreserve.gov/releases/h15/

[DGS10] Board of Governors of the Federal Reserve System (US), Federal Reserve Statistical Release H.15, Selected Interest Rates: U.S. Treasury securities, 10-year constant maturity, daily, percent (DDP series RIFLGFCY10_N.B), https://www.federalreserve.gov/releases/h15/ . Used only to calculate BREAKEVEN_10Y; not shipped as its own file.

[DTWEXBGS] Board of Governors of the Federal Reserve System (US), Federal Reserve Statistical Release H.10, Foreign Exchange Rates: Nominal Broad U.S. Dollar Index, daily, Jan 2006=100 (DDP series JRXWTFB_N.B), https://www.federalreserve.gov/releases/h10/

[CPIAUCSL] U.S. Bureau of Labor Statistics, Consumer Price Index for All Urban Consumers (CPI-U): All items in U.S. city average, seasonally adjusted, 1982-84=100, monthly (BLS series CUSR0000SA0, BLS Public Data API), https://www.bls.gov/cpi/

[UNRATE] U.S. Bureau of Labor Statistics, Labor Force Statistics from the Current Population Survey: Unemployment Rate, seasonally adjusted, percent, monthly (BLS series LNS14000000, BLS Public Data API), https://www.bls.gov/cps/

[PCEPI] U.S. Bureau of Economic Analysis, National Income and Product Accounts: Personal Consumption Expenditures, chain-type price index, 2017=100, seasonally adjusted, monthly (NIPA series DPCERG, NipaDataM.txt), https://apps.bea.gov/national/Release/TXT/NipaDataM.txt

[ICSA] U.S. Department of Labor, Employment and Training Administration, Unemployment Insurance Weekly Claims: national initial claims, seasonally adjusted, number of people, weekly ending Saturday (weekly claims data https://oui.doleta.gov/unemploy/claims.asp; newest weeks from the latest weekly news release https://www.dol.gov/ui/data.pdf)

Derived series BREAKEVEN_10Y: calculated by Tower from two of the series above:
  10-year breakeven inflation = DGS10 minus DFII10 (same day, percentage points).
  It is our own calculation, not a number published by the Federal Reserve.

Commitments of Traders (COT):
U.S. Commodity Futures Trading Commission, Commitments of Traders, Disaggregated Futures Only report,
GOLD - COMMODITY EXCHANGE INC. (contract market code 088691), https://publicreporting.cftc.gov (dataset 72hh-3qpy).
The CFTC dataset metadata names no required citation wording or licence; we credit the CFTC as the source.
Net managed-money position = managed-money long minus managed-money short; the week-over-week change is our calculation.
COT_GOLD_HISTORY.csv is built from the CFTC historical compressed files (fut_disagg_txt_YYYY.zip, https://www.cftc.gov/MarketReports/CommitmentsofTraders/HistoricalCompressed/index.htm). The change is versus the previous published report (holiday weeks shift the date).

This product is not endorsed by the Federal Reserve, the BLS, the BEA, the Employment and Training Administration or the CFTC.
```

## fed_forex

```
SOURCES AND CITATIONS - Forex Daily (Federal Reserve rates), daily pack
Data retrieved 2026-11-13 UTC.

All numbers come straight from the Federal Reserve Board: the H.10 'Foreign Exchange Rates' release and the Board's broad
dollar index, taken from the Board's Data Download Program (https://www.federalreserve.gov/datadownload/). The Board's data
is a US government work; we credit the Board as the source. Citation used for every series below:
Board of Governors of the Federal Reserve System (US), Federal Reserve Statistical Release H.10, Foreign Exchange Rates,
https://www.federalreserve.gov/releases/h10/ , series as named here.

[DEXUSEU] U.S. Dollars to Euro Spot Exchange Rate - Federal Reserve H.10 series RXI$US_N.B.EU
[DEXUSUK] U.S. Dollars to U.K. Pound Sterling Spot Exchange Rate - Federal Reserve H.10 series RXI$US_N.B.UK
[DEXUSAL] U.S. Dollars to Australian Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI$US_N.B.AL
[DEXUSNZ] U.S. Dollars to New Zealand Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI$US_N.B.NZ
[DEXJPUS] Japanese Yen to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.JA
[DEXCAUS] Canadian Dollars to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.CA
[DEXSZUS] Swiss Francs to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.SZ
[DEXCHUS] Chinese Yuan Renminbi to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.CH
[DEXKOUS] South Korean Won to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.KO
[DEXINUS] Indian Rupees to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.IN
[DEXMXUS] Mexican Pesos to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.MX
[DEXBZUS] Brazilian Reals to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.BZ
[DEXSDUS] Swedish Kronor to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.SD
[DEXSFUS] South African Rand to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.SF
[DEXTAUS] Taiwan Dollars to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.TA
[DEXHKUS] Hong Kong Dollars to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.HK
[DEXSIUS] Singapore Dollars to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.SI
[DEXNOUS] Norwegian Kroner to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.NO
[DEXDNUS] Danish Kroner to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.DN
[DEXTHUS] Thai Baht to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.TH
[DEXMAUS] Malaysian Ringgit to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.MA
[DEXSLUS] Sri Lankan Rupees to U.S. Dollar Spot Exchange Rate - Federal Reserve H.10 series RXI_N.B.SL
[DTWEXBGS] Nominal Broad U.S. Dollar Index - Federal Reserve H.10 series JRXWTFB_N.B

What the H.10 rates are: noon buying rates in New York City for cable transfers payable in foreign currencies, one
value per business day. They are published by the Federal Reserve, normally once a week (Monday, for the week before).
Pair names: EUR_USD, GBP_USD, AUD_USD and NZD_USD are US dollars per one euro / pound / Australian dollar / New Zealand
dollar. Every other pair USD_xxx is units of that currency per one US dollar. Values are exactly as published; we do not
invert, smooth, fill or round them. The ids (DEXUSEU and so on) are only our file names, kept from earlier packs.

This product is not endorsed by the Federal Reserve.
```
