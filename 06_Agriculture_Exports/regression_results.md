# Regression: Agriculture Production and Agricultural Exports

## Question and definition

This analysis asks whether faster growth in Uzbekistan's agricultural production is associated with faster growth in agricultural and food-related exports.

Export value is the sum of the National Statistics Committee's annual export categories with TN VED chapter codes 01–24. This includes food and processed agricultural products, fish, and tobacco; it is a broad trade measure, not a measure of exports of unprocessed farm output alone.

## Model

To reduce the risk of a misleading relationship caused by both nominal series rising over time, the model uses annual growth rates:

`Export growth (%)_t = 29.97 - 4.38 × Real agricultural production growth (%)_t + error_t`

The production predictor is the Committee's annual agricultural production growth index minus 100, so an index of 103.1 is entered as 3.1% growth. Export growth is calculated year over year from the annual export value totals in USD. The main regression uses 2011–2024 (14 observations); 2010 is the base year for calculating export growth.

## Results

| Statistic | Result |
|---|---:|
| Intercept | 29.97 |
| Production-growth coefficient | -4.38 |
| p-value for coefficient | 0.347 |
| R² | 0.074 |
| Observations | 14 |

The coefficient is not statistically significant at the 5% level. In this sample, a one-percentage-point higher real agricultural production growth rate is associated with a 4.38-percentage-point lower export growth rate, but the data do not provide reliable evidence of that relationship. The low R² also means this one-variable model explains little of the year-to-year variation in export growth.

## Limits

- Export values are nominal USD values, so world prices and exchange-rate changes can affect them even when exported quantities do not change.
- The export aggregate includes processed foods, fish, and tobacco, while the production indicator covers crops and livestock.
- The series is short. The export table notes final information through 2024, so 2025 is excluded from the regression.
- This is an association, not evidence that production growth causes export growth.

## Official sources

- [Agricultural production growth (annual), SIAT](https://siat.stat.uz/data/1454/?lang=en)
- [Agricultural production value (annual), SIAT](https://siat.stat.uz/data/1439/?lang=en)
- [Exports by 2-digit TN VED category (annual), SIAT](https://siat.stat.uz/data/3078/?lang=en)

Matched annual values are in `agriculture_production_exports_series.csv`. The original SIAT export download is preserved in `exports_by_commodity_annual.csv`.