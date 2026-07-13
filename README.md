# Portfolio Tracker 2.0

Official release repository for **Portfolio Tracker 2.0** — a Windows desktop application for managing, analysing, and optimising algorithmic trading strategy portfolios built with MultiWalk walkforward data.

## Download

| Version | Release date | Installer |
|---------|--------------|-----------|
| **v2.0.0** | 2026-07-13 | [PortfolioTracker-v2.0.0-Setup.exe](https://github.com/davidshuvalov/portfolio-tracker-releases/releases/download/v2.0.0/PortfolioTracker-v2.0.0-Setup.exe) |

Download from the [Releases](https://github.com/davidshuvalov/portfolio-tracker-releases/releases) page.

## System requirements

- **OS:** Windows 10 or Windows 11 (64-bit)
- **Dependencies:** None — the installer bundles everything required
- **Data:** MultiWalk walkforward project folders (or imported setup files)

## Install

1. Download `PortfolioTracker-v2.0.0-Setup.exe` from the table above or the [Releases](https://github.com/davidshuvalov/portfolio-tracker-releases/releases) page.
2. Double-click the installer.
3. Choose an install scope:
   - **All users** — installs to `Program Files`
   - **Just for me** — installs to `AppData`
4. Optionally create a desktop shortcut when prompted.

### Upgrading

To update an existing installation, download and run the new `Setup.exe`. The installer upgrades in place — no need to uninstall first.

## What is Portfolio Tracker 2.0?

Portfolio Tracker 2.0 is a complete rewrite of the original spreadsheet-based portfolio tracker. It is designed for systematic traders who run walkforward-optimised strategies via [MultiWalk](https://multiwalk.net/) and need a single tool to:

- **Track** dozens of strategies with status, contracts, margins, and performance metrics
- **Build** optimised portfolios with concentration, exposure, and margin constraints
- **Analyse** walkforward in-sample / out-of-sample results, Monte Carlo risk, and benchmark comparison
- **Size** contracts using margin and ATR multiples with micro/full contract switching
- **Export** PDF performance summaries for individual strategies and the full portfolio

The app integrates directly with MultiWalk project folders — import setup files, open ELCode, and navigate walkforward results without leaving the application.

## Key features (v2.0 initial release)

- **Portfolio Optimizer** — multi-step workflow with symbol/sector concentration rules, exposure limits, and Monte Carlo risk-of-ruin targeting
- **Strategy Tracker** — colour-coded status, contract-fit indicators, time-in-market, and auto-computed metrics
- **Walkforward Dashboard** — performance and inputs views with copy-ready parameter blocks
- **Monte Carlo simulation** — per-strategy and portfolio-level, with period selection (IS / OOS / all / last N years)
- **Contract Sizing** — margin and ATR multiple sliders with override support and decimal contract charts
- **Margin Tracking** — broker margin sources (TradeStation, Interactive Brokers, NinjaTrader) with reimport
- **Benchmark comparison** — alpha, beta, and correlation vs scaled buy-and-hold; Live Backtest reconstruction modes
- **Stress scenarios** — crisis replay and portfolio stress testing
- **Market Summary** — calendar analysis, market conditions, and strategy-vs-market views
- **Strategy Screener** — filter and action strategies by eligibility rules
- **PDF exports** — per-strategy and portfolio performance summaries
- **MultiWalk integration** — setup file import with automatic path rewriting when moving project folders

See [docs/v2.0.0-release-notes.md](docs/v2.0.0-release-notes.md) for the full v2.0.0 release notes and [CHANGELOG.md](CHANGELOG.md) for version history.

## Support

Portfolio Tracker is distributed to licensed users. For access, licensing, or support:

- **Email:** [davidshuvalov@gmail.com](mailto:davidshuvalov@gmail.com)

## Changelog

Release history is maintained in [CHANGELOG.md](CHANGELOG.md).
