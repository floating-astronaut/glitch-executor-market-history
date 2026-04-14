> **⚠️ FROZEN HISTORICAL ARCHIVE — as of 2026-04-14**
>
> This repository is no longer updated. All ML data collection now lives
> on the server at `/opt/ml/` and stays there — no new pushes land here.
>
> - **Authoritative live data:** PostgreSQL tables `ml_signals`, `ml_trades`,
>   `ml_bars` on the production server
> - **Daily CSV snapshots:** `/opt/ml/live/YYYY-MM-DD/` (systemd timer
>   `glitch-ml-export.timer`)
> - **Historical MT5-era archive** (what used to be pushed here): moved to
>   `/opt/ml/historical/` on the server
>
> Keep this repo around as read-only history. Archive in the GitHub UI
> when convenient (Settings → Danger Zone → Archive this repository).

---
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
