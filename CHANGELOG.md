# Changelog

All notable releases of Portfolio Tracker are documented here. Installers are published on the [Releases](https://github.com/davidshuvalov/portfolio-tracker-releases/releases) page.

## [2.4.2] — 2026-07-13

[Download](https://github.com/davidshuvalov/portfolio-tracker-releases/releases/download/v2.4.2/PortfolioTracker-v2.4.2-Setup.exe)

### Changed

- Margins: MultiWalk-only reference with custom overrides and reset; broker margin sources removed
- Recompute all portfolio-derived analytics when the portfolio changes
- Contract Sizing: Apply to Portfolio works without opening the Portfolio page first
- Strategy Compare: fix OOS view, add period options; Eligibility Rule Tester renamed and ungated
- Market Summary: returns shown as plain $ P&L per contract held
- Scaled P&L/ATR views, screener extras, compare period presets, margin-based returns
- Optimizer: randomised-search selection mode; inline Analyze sections; select-then-cull workflow
- Strategy MC: period selection with overlap rule
- Crisp text rendering for collapsed and expanded tables

## [2.4.1] — 2026-07-12

[Download](https://github.com/davidshuvalov/portfolio-tracker-releases/releases/download/v2.4.1/PortfolioTracker-v2.4.1-Setup.exe)

Maintenance release with the same feature set as 2.4.0. Rebuilt installer.

## [2.4.0] — 2026-07-12

[Download](https://github.com/davidshuvalov/portfolio-tracker-releases/releases/download/v2.4.0/PortfolioTracker-v2.4.0-Setup.exe)

### Added

- Optimizer: randomised-search selection mode to escape greedy local maxima
- Strategy MC: period selection (IS / OOS / all / last N years) with overlap rule
- Optimizer: inline Analyze sections that run on the result, not the portfolio
- Optimizer: select-then-cull, peak-daily margin basis, workflow MC defaults
- Optimizer: size from the ATR/margin formula by default; MC target downsize-only

### Changed

- Removed the optimizer's Historical Backtest tab
- Crisp text for collapsed tables (fixed-height scroll box, sticky header)
- Crisp HTML rendering for expanded tables (fix blurry canvas text)

### Fixed

- Crash-safe import, un-skipped integration tests, atomic settings restore

## [2.0.0] — 2026-07-05

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
