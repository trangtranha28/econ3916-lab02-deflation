# Deflating Economic Data — Nominal vs. Real

**Objective:** This project analyzes U.S. wage and price data from FRED to distinguish nominal changes from real, inflation-adjusted changes, illustrating how apparent economic gains can be partially or fully offset by inflation.

**Methodology:**
- Retrieved CPI and average hourly earnings series from the FRED API (no key required)
- Implemented a `deflate_series()` function to convert nominal values into constant [BASE_YEAR] dollars
- Applied the deflator to both wage data and Big Mac price data to compare nominal vs. real trends
- Calculated percentage changes in nominal price, real (deflated) price, and CPI over the same time window
- Built an interactive deflation explorer allowing users to adjust the base year via a slider and observe how real values shift

**Key Findings:**
- Nominal hourly earnings rose from [NOMINAL_START] to [NOMINAL_END] between [START_DATE] and [END_DATE]
- After adjusting for inflation, real hourly earnings moved from [REAL_START] to [REAL_END] over the same period
- The U.S. Big Mac price increased [NOMINAL_PCT]% in nominal terms but only [REAL_PCT]% in real terms, against a CPI increase of [CPI_PCT]%
- The gap between nominal and real changes highlights the extent to which inflation eroded purchasing power over the period studied
