# Uzbekistan Gold Exports — Research Data

Collected: 18 November 2026.

## Start here
- 00_Start_Here/Gold_Exports_Annual_2017_2025.csv: a derived table from WITS World totals, with export value converted from thousands of USD to USD, quantities in kg and tonnes, and annual value growth. Nine annual observations.
- 00_Start_Here/Gold_Prices_and_Exports_Annual_1996_2025.csv: a 30-year comparison panel of annual gold prices and available gold export values. Export fields are blank where the current WITS dataset has no observation; blanks do not mean zero.
- 00_Start_Here/Gold_Prices_Annual_USD_per_troy_ounce.csv and Gold_Prices_Monthly_USD_per_troy_ounce.csv: nominal gold prices extracted from the original World Bank Excel workbooks.

## Original data and reports
- 01_Uzbekistan_Statistics: full export-structure monthly table, annual goods-export totals and monthly export totals in CSV/XLSX/JSON; official 2025 foreign trade report. These are general trade datasets, not all gold-only tables.
- 02_WITS_UN_Comtrade: original WITS HTML pages requested for 2010–2025, CSV transcriptions for years with records (2017–2025), and a combined partner table.
- 03_World_Bank_Prices: full annual and monthly historical commodity workbooks plus all distinct 2026 Pink Sheet PDFs linked on the cited page at collection time (February–November). Gold-only annual and monthly CSV extracts are supplied for convenience.
- 04_Central_Bank: statistical bulletin dated 1 July 2026 and 2025 balance-of-payments report. Supporting context, not a substitute for gold exports.
- 05_Source_Pages: source-page HTML snapshots for provenance; some Central Bank category URLs returned the general Statistics page.

## Coverage and access limitations
The new 1996–2025 comparison panel has 30 annual rows, but Uzbekistan gold-export observations remain available in the current WITS files only for 2017–2025. WITS pages for 2010–2016 returned no data table, and earlier gold-export values were not verified in the sources collected here. Missing data are not zero exports. Do not use the 30-year panel as a 30-year gold-export regression dataset until historical export values are obtained from a reliable source.
This package collects relevant public downloads from the nine previously listed links and associated downloads, not every dataset on those institutions' websites.
Direct UN Comtrade bulk/history requests returned HTTP 429 (rate limiting), and one request returned HTTP 400. No direct UN API historical dataset was obtained. Use WITS files here for the available annual history; WITS republishes UN Comtrade and is not independent confirmation.
The WITS country-partner CSV contains both World totals and individual partners: do not sum World together with partner rows. Unspecified destinations must not be assigned to countries.
WITS classification is HS 1988/92 code 7108 (broad gold category), not a single narrowly defined non-monetary gold subheading. Quantity values are displayed rounded and may be estimated by the original provider. Retain source caveats.
National and WITS totals can differ because of classification, scope, timing and revisions; do not force them to match. Check dataset metadata and units before calculating gold shares. Monthly national figures may be cumulative year-to-date.
2026 observations are partial-year and must not be compared directly with complete annual figures.

## Source URLs
1. https://wits.worldbank.org/trade/comtrade/en/country/UZB/year/2025/tradeflow/Exports/partner/ALL/product/7108
2. https://comtradeplus.un.org/en/
3. https://stat.uz/en/official-statistics/merchandise-trade
4. https://siat.stat.uz/data/3082/?lang=en
5. https://siat.stat.uz/data/1143/?lang=en
6. https://siat.stat.uz/data/1103/?lang=en
7. https://stat.uz/img/news/4_-talil-2025-j_-yanvar-dekabr-angl-_p47537.pdf
8. https://thedocs.worldbank.org/en/doc/74e8be41ceb20fa0da750cda2f6b9e4e-0050012026/world-bank-commodities-price-data-the-pink-sheet
9. https://cbu.uz/en/statistics/

See download_log.json for individual successful and failed requests and validation.json for verified Excel workbook structure. CSV transcriptions/derived files are separate from original publisher downloads.
