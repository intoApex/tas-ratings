# TAS Ratings: risk scores for AI agents that touch money

Open data from [TradingAgentStack](https://tradingagentstack.com). One question drives every score: **if the agent is wrong, hacked or prompt-injected, how much money can it lose?**

- **35 Agent Risk Scores** for agent wallets, exchanges for bots, on-chain and DeFi agents, agent payment rails, AI trading agents and agent tokens with a real product
- **140 tools** in the full directory, with sources and last-checked dates
- **6 incidents** from official disclosures

Generated 2026-10-26 from the live site. Updated automatically on every site release; do not edit by hand.

## Files

| File | What it is |
|---|---|
| `data/agent-risk-scores.json` / `.csv` | Every Agent Risk Score with each input's points, note and official source |
| `data/incidents.json` | The incident tracker |
| `data/tools.json` / `.csv` | The full directory, including the older safety score for broker tools |
| `guard-profiles/` | TAS Guard connector profiles (which tools of a broker MCP server place, change or cancel orders) |

## How the score works

Seven inputs, 100 points: custody (20), limits enforced outside the model (20), human approval (15), withdrawal and transfer scope (15), preview or simulation (10), open source and audits (10), track record and sourcing (10). Every point links to the vendor's own docs. **Missing inputs are shown as missing, not zero, and lower the maximum** (those scores are marked partial). No paid scores; affiliate links are never read by the scoring code. Full method: https://tradingagentstack.com/methodology/

## Current scores

### AI agent payments

| Tool | Agent Risk Score | Missing inputs |
|---|---|---|
| [Link agent wallet](https://tradingagentstack.com/tool/link-agent-wallet/#agent-risk-score) | 84% (partial) | preview |
| [Agent Payments Protocol (AP2)](https://tradingagentstack.com/tool/agent-payments-protocol-ap2/#agent-risk-score) | 69% (partial) | custody, limits, withdraw, preview |
| [Stripe Issuing for agents](https://tradingagentstack.com/tool/stripe-issuing-for-agents/#agent-risk-score) | 56% (partial) | preview |
| [Lightning Agent Tools](https://tradingagentstack.com/tool/lightning-agent-tools/#agent-risk-score) | 52% (partial) | approval, withdraw, preview |
| [x402](https://tradingagentstack.com/tool/x402/#agent-risk-score) | 52% (partial) | custody, approval, withdraw, preview |
| [Coinbase Agentic Wallet](https://tradingagentstack.com/tool/coinbase-agentic-wallet/#agent-risk-score) | 51% (partial) | preview |

### AI agent wallets

| Tool | Agent Risk Score | Missing inputs |
|---|---|---|
| [Safe Smart Account](https://tradingagentstack.com/tool/safe-smart-account/#agent-risk-score) | 100% (partial) | preview |
| [ZeroDev](https://tradingagentstack.com/tool/zerodev/#agent-risk-score) | 88% (partial) | approval, preview |
| [Crossmint Agent Wallets](https://tradingagentstack.com/tool/crossmint-agent-wallets/#agent-risk-score) | 67% (partial) | preview |
| [Turnkey](https://tradingagentstack.com/tool/turnkey/#agent-risk-score) | 64% (partial) | preview |
| [Privy server wallets](https://tradingagentstack.com/tool/privy-server-wallets/#agent-risk-score) | 63% | none |
| [Coinbase CDP Server Wallets](https://tradingagentstack.com/tool/coinbase-cdp-server-wallets/#agent-risk-score) | 56% (partial) | preview |
| [Coinbase AgentKit](https://tradingagentstack.com/tool/coinbase-agentkit/#agent-risk-score) | 38% (partial) | preview |

### AI trading agents

| Tool | Agent Risk Score | Missing inputs |
|---|---|---|
| [Binance Agentic Wallet](https://tradingagentstack.com/tool/binance-agentic-wallet/#agent-risk-score) | 69% | none |
| [Bitget Wallet Skill](https://tradingagentstack.com/tool/bitget-wallet-skill/#agent-risk-score) | 60% (partial) | limits, withdraw |
| [HeyAnon](https://tradingagentstack.com/tool/heyanon/#agent-risk-score) | 55% (partial) | custody, limits |
| [OKX Agentic Wallet](https://tradingagentstack.com/tool/okx-agentic-wallet/#agent-risk-score) | 46% (partial) | limits, withdraw |

### Agent tokens with a product

| Tool | Agent Risk Score | Missing inputs |
|---|---|---|
| [Virtuals ACP (acp-cli)](https://tradingagentstack.com/tool/virtuals-acp-acp-cli/#agent-risk-score) | 84% (partial) | preview |
| [Olas Pearl](https://tradingagentstack.com/tool/olas-pearl/#agent-risk-score) | 46% (partial) | custody, limits, withdraw, preview |

### Exchanges & brokers for bots

| Tool | Agent Risk Score | Missing inputs |
|---|---|---|
| [Bybit](https://tradingagentstack.com/tool/bybit/#agent-risk-score) | 89% (partial) | limits |
| [Binance](https://tradingagentstack.com/tool/binance/#agent-risk-score) | 86% (partial) | limits, preview |
| [OKX](https://tradingagentstack.com/tool/okx/#agent-risk-score) | 84% (partial) | limits, preview |
| [Bitget](https://tradingagentstack.com/tool/bitget/#agent-risk-score) | 80% (partial) | limits |
| [Kraken](https://tradingagentstack.com/tool/kraken/#agent-risk-score) | 76% | none |
| [Coinbase Advanced](https://tradingagentstack.com/tool/coinbase-advanced/#agent-risk-score) | 72% (partial) | limits |
| [Gemini](https://tradingagentstack.com/tool/gemini/#agent-risk-score) | 70% (partial) | limits |
| [Hyperliquid](https://tradingagentstack.com/tool/hyperliquid/#agent-risk-score) | 64% (partial) | limits, preview |

### On-chain & DeFi trading agents

| Tool | Agent Risk Score | Missing inputs |
|---|---|---|
| [0x Swap API](https://tradingagentstack.com/tool/0x-swap-api/#agent-risk-score) | 75% (partial) | limits, approval, withdraw, preview |
| [Jupiter API](https://tradingagentstack.com/tool/jupiter-api/#agent-risk-score) | 75% (partial) | limits, approval, withdraw, preview |
| [1inch Swap API](https://tradingagentstack.com/tool/1inch-swap-api/#agent-risk-score) | 69% (partial) | limits, withdraw, preview |
| [BONKbot](https://tradingagentstack.com/tool/bonkbot/#agent-risk-score) | 50% (partial) | custody, limits, approval, withdraw, preview |
| [Banana Gun](https://tradingagentstack.com/tool/banana-gun/#agent-risk-score) | 50% (partial) | custody, limits, approval, withdraw, preview |
| [Solana Agent Kit](https://tradingagentstack.com/tool/solana-agent-kit/#agent-risk-score) | 40% (partial) | limits, approval, withdraw, preview |
| [Maestro](https://tradingagentstack.com/tool/maestro/#agent-risk-score) | 18% (partial) | limits, approval, preview |
| [Trojan](https://tradingagentstack.com/tool/trojan/#agent-risk-score) | 18% (partial) | limits, approval, preview |

## Use it

- Download the JSON or CSV above, or read it live from `https://tradingagentstack.com/data/tools.json`.
- From an AI agent: the TradingAgentStack MCP server (`npx -y tradingagentstack-mcp`, or `https://tradingagentstack.com/api/mcp`) has `get_risk` and `get_incidents`.

## Corrections

Found a wrong fact? Open an issue with a link to the vendor's official docs, or use https://tradingagentstack.com/submit/. Facts without an official source aren't added.

## License

Data: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Credit "TradingAgentStack (tradingagentstack.com)". Not financial advice; verify with the vendor.
