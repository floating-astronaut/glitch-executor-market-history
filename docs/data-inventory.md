# Data Inventory

## Summary

- Approximate size: `0.94 GB`
- Total files: `46`

## Included Sources

- `raw/gold`
  - XAU intraday and higher-timeframe files
  - `XAU_1m_data.csv` preserved as `XAU_1m_parts/`
- `raw/eurusd_m1`
  - EURUSD M1 yearly archive CSVs
- `raw/btc`
  - BTC historical daily and intraday source files
- `raw/oil`
  - Brent and WTI reference price files

## Notable Files

- `raw/gold/XAU_5m_data.csv`
- `raw/gold/XAU_15m_data.csv`
- `raw/gold/XAU_1m_parts/XAU_1m_part_001.csv` through `XAU_1m_part_005.csv`
- `raw/btc/btc_usd_5m_bitstamp_18-08-2011_27-04-2021.csv`
- `raw/btc/bitcoin_2010-07-17_2024-05-23.csv`
- `raw/btc/bitcoin_2010-07-17_2024-06-28.csv`

## Exclusions

- account-specific CSV exports from the old archive
- duplicate `.txt` versions of the EURUSD files
- mixed logs and non-market artifacts from the larger archive folder
