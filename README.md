# Glitch Executor Market History

Private historical market-data repository for the Glitch Executor ecosystem.

This repository preserves raw external time-series datasets used for research, backtesting, data-engineering, and archive retention. It exists so large historical market files can stay isolated from the public code repos and from the model/data repos that hold Glitch-specific training assets.

## Repo Role

This repo is the market-history archive. It is intended to preserve:

- raw XAU historical data
- EURUSD M1 archives
- BTC history snapshots
- supporting oil or macro reference price files

## Structure

- `raw/` for source market-history files grouped by asset family
- `docs/` for inventory, handling notes, and archive decisions

## Privacy

This repository should remain private.

Even though the files are market data rather than credentials, this repo is still part of the private Glitch research estate and should not be mirrored casually.

## Notes

- oversized source files may be split into smaller archive parts to stay inside normal GitHub limits
- account-specific exports do not belong here unless they are explicitly sanitized and research-relevant
- this repo should contain raw reference data, not strategy code or model artifacts
