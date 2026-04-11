# Glitch Executor Market History

Private raw market-history repository for the Glitch Executor ecosystem.

This repo preserves external historical market datasets that are useful for research, backtesting, and future data-engineering work, but do not belong in the public code repos.

## Purpose

This repository exists to preserve:

- raw XAU historical time-series files
- raw EURUSD M1 historical archives
- BTC historical market datasets
- supporting oil reference price files

## Privacy Rule

This repository should remain private.

## Current Payload

- Approximate size: `0.94 GB`
- Total files: `46`

## Structure

```text
glitch-executor-market-history/
|-- raw/
|   |-- gold/
|   |-- eurusd_m1/
|   |-- btc/
|   `-- oil/
`-- docs/
```

## Notes

- The oversized `XAU_1m_data.csv` source file was split into `raw/gold/XAU_1m_parts/` to stay within normal GitHub file-size limits without relying on Git LFS.
- The `EURUSD` archive preserves only the CSV time-series files, not the adjacent `.txt` duplicates.
- Account-specific CSV files from the old archive were intentionally excluded because they are not raw market-history assets.
