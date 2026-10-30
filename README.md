# JadeFox (捷狐投研)

> **High-Performance, Local-First Quantitative Financial Analysis & AI Investment Research Desktop Workbench.**

[![GitHub Release](https://img.shields.io/github/v/release/xtc002007/JadeFox?style=flat-square&color=emerald)](https://github.com/xtc002007/JadeFox/releases)
[![Platform](https://img.shields.io/badge/platform-Windows%20x64-blue.svg?style=flat-square)](https://nexustools.tech)
[![Engine](https://img.shields.io/badge/backend-Rust%20%7C%20Tauri%20v2-orange.svg?style=flat-square)](https://tauri.app)
[![UI](https://img.shields.io/badge/frontend-React%2019%20%7C%20Tailwind-61dafb.svg?style=flat-square)](https://react.dev)
[![License](https://img.shields.io/badge/license-Proprietary-lightgrey.svg?style=flat-square)](./LICENSE)

---

## 📌 Overview

**JadeFox (捷狐投研)** is an AI-native, high-performance financial quantitative research and investment decision workbench built for serious equity investors, quants, and market analysts. Engineered on a modern **Rust + Tauri v2 + React 19** architecture, JadeFox combines real-time streaming market data, local embedded analytical databases, multi-factor quantitative screening, and deep LLM-powered financial auditing.

This repository serves as the **official public distribution and release portal** for JadeFox binaries, release notes, and automated package management manifests (including the [Windows Package Manager](https://github.com/microsoft/winget-pkgs)).

---

## ⚡ Key Highlights & Core Capabilities

### 1. Real-Time Market Overview & Sentiment Streaming
- **Level-1/Level-2 Market Feeds**: Low-latency streaming of A-share ticks, intraday bid/ask books, and real-time turnover rates.
- **Market Sentiment Heatmaps**: Dynamic sector heatmaps, market breadth gauges, daily advance/decline distribution, and real-time capital flow trackers (Northbound / Southbound funds).
- **Macro & Flash News Aggregator**: Real-time regulatory filings, exchange disclosures, and financial wire events tagged with entity recognition.

### 2. High-Performance Local Financial Computing Engine
- **Local-First Zero-Privacy Leakage**: Your watchlists, custom factors, notes, and trading journals are stored exclusively on your local machine in embedded SQLite databases (`market.db`, `fundamental.db`, `factor.db`, `user.db`, `knowledge.db`).
- **Rust-Powered Computation**: Multi-threaded technical indicator calculations (MACD, KDJ, RSI, Bollinger Bands, ATR) and financial statement parsing executed in sub-millisecond native Rust code.

### 3. Multi-Factor Quantitative Strategy Screener
- **Comprehensive Factor Library**: Valuation metrics (PE-TTM, PB, PS, PCF, EV/EBITDA), profitability factors (ROE, ROIC, Gross Margin, Net Margin), solvency indicators, and momentum indicators.
- **Custom Factor Combinations**: Multi-condition boolean filtering, percentile ranking, and customizable screening templates.
- **Automated Universe Filtering**: Filter across 5,000+ equities in fractions of a second without sending requests to external web servers.

### 4. AI Stock Research Terminal (10-Section Deep Audit)
- **Deep Automated Fundamental Analysis**: Generates comprehensive institutional-grade research dossiers covering business models, competitive moats, unit economics, supply-chain positioning, and growth catalysts.
- **Multi-Model LLM Support**: Native BYOK (Bring Your Own Key) integration for **DeepSeek (V3/R1)**, **OpenAI (GPT-4o/o1)**, and **Anthropic (Claude 3.5 Sonnet)**.
- **Secure Key Storage**: API tokens are encrypted and secured via your operating system's native Credential Manager / Keychain.

### 5. Value Trap & Forensic Accounting Detector (12 Heuristic Rules)
- **Anti-Fraud Auditing Engine**: Evaluates corporate disclosures against 12 proven financial fraud indicators:
  - Divergence between revenue growth and accounts receivable
  - Gross margin anomalies compared to industry peers
  - Operating cash flow vs. net profit discrepancies
  - Excessive collateralized equity ratios by controlling shareholders
  - Frequent auditor replacements and qualified audit opinions
  - Hidden liabilities, goodwill impairment risk, and off-balance-sheet commitments

### 6. Master Perspectives & Mental Models
- **6 Classical Investment Frameworks**: Analyze any company through the specialized qualitative mental models of investment legends:
  - **Warren Buffett**: Durable competitive moat, owner earnings, return on capital, management integrity.
  - **Peter Lynch**: Tenbagger categorization (fast growers, stalwarts, turnarounds, cyclicals), peg ratio.
  - **Benjamin Graham**: Deep value, net-current-asset value (NCAV), margin of safety.
  - **Charlie Munger**: Lollapalooza effects, inversion, competitive destruction risks.
  - **Philip Fisher**: 15-point scuttlebutt methodology, R&D productivity.
  - **Howard Marks**: Market cycle positioning, second-order thinking, asymmetric risk.

### 7. Pre-Trade Decision Center & Investment Journal
- **Discipline Checklists**: Pre-configured buy/sell gatekeepers to prevent emotional trading and fomo behavior.
- **AI Performance Coach**: Automatic trade logging, behavioral post-mortems, and cognitive bias detection over time.

---

## 🚀 Installation & Downloads

### Method 1: Windows Package Manager (winget) — Recommended

Install JadeFox with a single command via Windows Terminal or PowerShell:

```powershell
winget install NexusTools.JadeFox
```

To update an existing installation to the latest release:

```powershell
winget upgrade NexusTools.JadeFox
```

---

### Method 2: Direct Download from GitHub Releases

Visit the [Latest GitHub Releases](https://github.com/xtc002007/JadeFox/releases/latest) page to download official binaries:

| Package Asset | Description | Recommended For |
| :--- | :--- | :--- |
| `JadeFox_<version>_windows_x64_setup.exe` | Standard Windows NSIS Installer | All users (enables desktop integration & auto-updates) |
| `JadeFox_<version>_windows_x64_portable.zip` | Standalone Portable Archive | Portable USB drives or environments without admin rights |

---

### Method 3: Official NexusTools Portal

Download and manage JadeFox along with the entire NexusTools productivity suite at [https://nexustools.tech](https://nexustools.tech).

---

## 🔒 Security, Authenticity & Verification

Every JadeFox release is cryptographically protected against tampering:
- **Minisign (Ed25519) Signatures**: Every `.exe` release includes a companion `.sig` signature file verifying authentic builds.
- **Windows Authenticode Signing**: Binaries are digitally signed to guarantee code provenance.
- **Silent Background Updates**: Integrated silent auto-updater queries HTTPS endpoints over TLS 1.3 with cryptographic manifest validation.

---

## ⚖️ License & EULA

JadeFox is distributed under the [NexusTools End-User License Agreement (EULA)](./LICENSE).
- Core fundamental viewing, local screener, and personal watchlist features are permanently free for personal research.
- Advanced AI synthesis and real-time cloud capabilities are governed by the unified NexusTools account tier.

> **Disclaimer**: JadeFox is an objective financial research and analytical tool. It does NOT provide individualized investment advice or buy/sell execution services. All algorithmic outputs and AI summaries are for informational purposes only.

---

## 💬 Community & Support

- **Bug Reports & Feature Requests**: [GitHub Issues](https://github.com/xtc002007/JadeFox/issues)
- **Official Website & Docs**: [https://nexustools.tech](https://nexustools.tech)
- **NexusTools Ecosystem**: Part of the [NexusTools Desktop Suite](https://github.com/xtc002007).
