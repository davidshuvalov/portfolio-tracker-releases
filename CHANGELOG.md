# Changelog

All notable releases of Portfolio Tracker are documented here. Installers are published on the [Releases](https://github.com/davidshuvalov/portfolio-tracker-releases/releases) page.

## [2.0.1] — 2026-07-13

**Initial public release.** First release of Portfolio Tracker 2.0 to licensed users.

[Download](https://github.com/davidshuvalov/portfolio-tracker-releases/releases/download/v2.0.1/PortfolioTracker-v2.0.1-Setup.exe)

See [docs/v2.0.1-release-notes.md](docs/v2.0.1-release-notes.md) for the full release notes.

### Fixed

- Fixed Portfolio at a Glance widget to properly use configured status options

## [2.0.0] — 2026-07-13

**Initial Portfolio Tracker 2.0 release.** Restarts the release line with a standalone Windows installer.

[Download](https://github.com/davidshuvalov/portfolio-tracker-releases/releases/download/v2.0.0/PortfolioTracker-v2.0.0-Setup.exe)

See [docs/v2.0.0-release-notes.md](docs/v2.0.0-release-notes.md) for the full release notes.

### Added

- Portfolio Optimizer with concentration rules, exposure limits, and MC risk-of-ruin targeting
- Strategy Tracker with colour-coded status, contract-fit indicators, and time-in-market
- Walkforward Dashboard (Performance and Inputs tabs)
- Per-strategy and portfolio Monte Carlo simulation
- Contract Sizing with margin/ATR multiples and decimal contract charts
- Margin Tracking with TradeStation, IB, and NinjaTrader sources
- Portfolio vs Benchmark (alpha/beta/correlation)
- Stress Scenario / Crisis Replay page
- Benchmark with Live Backtest reconstruction modes
- Market Summary with Calendar Analysis
- Strategy Screener and Eligibility Backtest
- PDF performance-summary exports
- MultiWalk setup file import with automatic path rewriting
- ELCode and folder quick-open buttons
- Expand/Collapse toggle on all tables
- Configurable status options with colour coding
- Official logo design pack (candlestick icon + gold wordmark)

### Changed

- Complete rewrite from the original Excel-based Portfolio Tracker workbook
- Standalone Windows installer — no Python runtime required

### Fixed

- ATR Rebalance crash on flat (zero-range) days
- Optimizer over-sizing: margin cap on MC target, full-margin basis, micro rule
- Concentration rule cascade: absolute % of equity not % of portfolio
- Stale row selection and strategy name resolution in tables
- Segfaults in ATR computation on CI (pandas datetime handling)
