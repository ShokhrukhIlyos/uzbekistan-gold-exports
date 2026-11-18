# Uzbekistan Mining Production Factors

Annual Uzbekistan data extracted from SIAT tables published by the National Statistics Committee. Coverage is 2010–2025 (16 rows per series).

## Files

- `investment_fixed_assets_mining_quarrying.csv` — investment in fixed assets in mining and quarrying; billion UZS. [SIAT indicator 1.04.01.0070](https://siat.stat.uz/data/1899/?lang=en)
- `foreign_investment_mining_quarrying.csv` — foreign investment and loans in mining and quarrying; billion UZS. [SIAT indicator 1.04.01.0027](https://siat.stat.uz/data/1902/?lang=en)
- `mining_quarrying_employment.csv` — employed population in mining and quarrying; thousand people. [SIAT indicator 2.02.01.1500](https://siat.stat.uz/data/1315/?lang=en)
- `electricity_production_uzbekistan.csv` — total national electricity production; million kWh. This is not gold-mine electricity consumption. [SIAT indicator 1.02.02.0004](https://siat.stat.uz/data/440/?lang=en)
- `mining_quarrying_gva_constant_prices.csv` — mining and quarrying gross value added; billion UZS at previous-year prices. [SIAT indicator 1.01.01.0006](https://siat.stat.uz/data/1209/?lang=en)

## Notes for analysis

- The 2025 employment and electricity observations are marked preliminary by SIAT.
- The employment series has a sharp level change between 2016 and 2017; check for a classification or measurement break before using it.
- Investment amounts are nominal. Deflate them before interpreting changes as real investment.
- Foreign mining investment is a component of the broader mining investment measure. Avoid including both in the same regression without checking collinearity.
- Mining value added covers more than gold and includes gold production itself, so it can overlap mechanically with the dependent variable.
- The gold-production series currently used in the project covers 2010–2024. This leaves at most 15 common annual observations before applying lags; a 1-year lag leaves 14.
- These are sector-wide or national proxies, not gold-mine-specific records. Do not interpret their regression coefficients as causal effects.

SIAT source pages list CC BY 4.0. The CSVs preserve annual values, units, source links, and brief notes.
