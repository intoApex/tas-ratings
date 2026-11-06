# TAS Ratings: risk scores for AI agents that touch money

Open data from [TradingAgentStack](https://tradingagentstack.com). One question drives every score: **if a tool, or an AI agent using it, is wrong, hacked or prompt-injected, how much money can it lose?**

- **164 Safety scores**, one for every tool in the directory: agent wallets, exchanges for bots, on-chain and DeFi agents, agent payment rails, AI trading agents, broker MCP servers, bots and more, with sources and last-checked dates
- **20 incidents** from official disclosures

Generated 2026-11-06 from the live site. Updated automatically on every site release; do not edit by hand.

## Files

| File | What it is |
|---|---|
| `data/safety-scores.json` / `.csv` | Every Safety score with each input's points, note and source |
| `data/agent-risk-scores.json` / `.csv` | Deprecated: the crypto agent tools only, with the old Agent Risk Score input names; equal to the Safety score since 2026-11-01 |
| `data/incidents.json` | The incident tracker |
| `data/tools.json` / `.csv` | The full directory, with the Safety score fields |
| `guard-profiles/` | TAS Guard connector profiles (which tools of a broker MCP server place, change or cancel orders) |

## How the score works

Seven inputs, 100 points: human approval (25), guardrails outside the agent (15), test before real money (15), sending funds out (15), who holds the keys (10), open source or audited (10), incident record in the last 12 months (10). Each input uses an owner-approved correction first, then a fact from the vendor's official docs, then the listing. **Missing inputs are shown as missing, not zero, and lower the maximum** (those scores are marked partial). Since 2026-11-01 this one score replaces the separate Agent Risk Score. No paid scores; affiliate links are never read by the scoring code. Full method: https://tradingagentstack.com/methodology/

## Current scores

### AI agent payments

| Tool | Safety score | Missing inputs |
|---|---|---|
| [Agent Payments Protocol (AP2)](https://tradingagentstack.com/tool/agent-payments-protocol-ap2/#safety) | 75% (partial) | paper, withdraw, keys |
| [Link agent wallet](https://tradingagentstack.com/tool/link-agent-wallet/#safety) | 75% | none |
| [x402](https://tradingagentstack.com/tool/x402/#safety) | 64% (partial) | keys |
| [Lightning Agent Tools](https://tradingagentstack.com/tool/lightning-agent-tools/#safety) | 56% (partial) | withdraw |
| [Coinbase Agentic Wallet](https://tradingagentstack.com/tool/coinbase-agentic-wallet/#safety) | 55% | none |
| [Stripe Issuing for agents](https://tradingagentstack.com/tool/stripe-issuing-for-agents/#safety) | 55% | none |

### AI agent wallets

| Tool | Safety score | Missing inputs |
|---|---|---|
| [Safe Smart Account](https://tradingagentstack.com/tool/safe-smart-account/#safety) | 100% | none |
| [ZeroDev](https://tradingagentstack.com/tool/zerodev/#safety) | 70% | none |
| [Coinbase AgentKit](https://tradingagentstack.com/tool/coinbase-agentkit/#safety) | 65% | none |
| [Privy server wallets](https://tradingagentstack.com/tool/privy-server-wallets/#safety) | 65% | none |
| [Turnkey](https://tradingagentstack.com/tool/turnkey/#safety) | 65% | none |
| [Crossmint Agent Wallets](https://tradingagentstack.com/tool/crossmint-agent-wallets/#safety) | 60% | none |
| [Coinbase CDP Server Wallets](https://tradingagentstack.com/tool/coinbase-cdp-server-wallets/#safety) | 55% | none |

### AI signals & research copilots

| Tool | Safety score | Missing inputs |
|---|---|---|
| [Danelfin](https://tradingagentstack.com/tool/danelfin/#safety) | 90% | none |
| [Intellectia](https://tradingagentstack.com/tool/intellectia/#safety) | 90% | none |
| [Kaito](https://tradingagentstack.com/tool/kaito/#safety) | 90% | none |
| [Kavout](https://tradingagentstack.com/tool/kavout/#safety) | 90% | none |
| [LevelFields](https://tradingagentstack.com/tool/levelfields/#safety) | 90% | none |
| [LunarCrush](https://tradingagentstack.com/tool/lunarcrush/#safety) | 90% | none |
| [Nansen](https://tradingagentstack.com/tool/nansen/#safety) | 90% | none |
| [Prospero.ai](https://tradingagentstack.com/tool/prospero-ai/#safety) | 90% | none |
| [Santiment](https://tradingagentstack.com/tool/santiment/#safety) | 90% | none |

### AI trading agents

| Tool | Safety score | Missing inputs |
|---|---|---|
| [Binance Agentic Wallet](https://tradingagentstack.com/tool/binance-agentic-wallet/#safety) | 65% | none |
| [Mangrove](https://tradingagentstack.com/tool/mangrove/#safety) | 58% | none |
| [HeyAnon](https://tradingagentstack.com/tool/heyanon/#safety) | 56% (partial) | keys |
| [Bitget Wallet Skill](https://tradingagentstack.com/tool/bitget-wallet-skill/#safety) | 55% | none |
| [Tria Agentic Trading](https://tradingagentstack.com/tool/tria-agentic-trading/#safety) | 35% | none |
| [OKX Agentic Wallet](https://tradingagentstack.com/tool/okx-agentic-wallet/#safety) | 25% | none |

### AI trading bot platforms

| Tool | Safety score | Missing inputs |
|---|---|---|
| [TradersPost](https://tradingagentstack.com/tool/traderspost/#safety) | 72% (partial) | keys |
| [3Commas](https://tradingagentstack.com/tool/3commas/#safety) | 58% | none |
| [Nova Trading App](https://tradingagentstack.com/tool/nova-trading-app/#safety) | 53% (partial) | keys |
| [Option Alpha](https://tradingagentstack.com/tool/option-alpha/#safety) | 53% (partial) | keys |
| [Nyria](https://tradingagentstack.com/tool/nyria/#safety) | 51% (partial) | withdraw |
| [Bitsgap](https://tradingagentstack.com/tool/bitsgap/#safety) | 50% | none |
| [Coinrule](https://tradingagentstack.com/tool/coinrule/#safety) | 50% | none |
| [Cryptohopper](https://tradingagentstack.com/tool/cryptohopper/#safety) | 50% | none |
| [Surmount](https://tradingagentstack.com/tool/surmount/#safety) | 50% | none |
| [WunderTrading](https://tradingagentstack.com/tool/wundertrading/#safety) | 50% | none |
| [Capitalise.ai](https://tradingagentstack.com/tool/capitalise-ai/#safety) | 33% (partial) | withdraw, keys |
| [Tickeron](https://tradingagentstack.com/tool/tickeron/#safety) | 33% (partial) | withdraw, keys |
| [Trade Ideas (Holly AI)](https://tradingagentstack.com/tool/trade-ideas-holly-ai/#safety) | 33% (partial) | withdraw, keys |
| [Composer](https://tradingagentstack.com/tool/composer/#safety) | 29% (partial) | paper |
| [Pionex](https://tradingagentstack.com/tool/pionex/#safety) | 24% (partial) | paper |
| [TrendSpider](https://tradingagentstack.com/tool/trendspider/#safety) | 17% (partial) | paper, withdraw, keys |

### Agent frameworks

| Tool | Safety score | Missing inputs |
|---|---|---|
| [LangGraph](https://tradingagentstack.com/tool/langgraph/#safety) | 100% | none |
| [LlamaIndex](https://tradingagentstack.com/tool/llamaindex/#safety) | 100% | none |
| [Mastra](https://tradingagentstack.com/tool/mastra/#safety) | 100% | none |
| [Microsoft Agent Framework](https://tradingagentstack.com/tool/microsoft-agent-framework/#safety) | 100% | none |
| [TradingAgents](https://tradingagentstack.com/tool/tradingagents/#safety) | 100% | none |

### Agent tokens with a product

| Tool | Safety score | Missing inputs |
|---|---|---|
| [Virtuals ACP (acp-cli)](https://tradingagentstack.com/tool/virtuals-acp-acp-cli/#safety) | 95% | none |
| [Olas Pearl](https://tradingagentstack.com/tool/olas-pearl/#safety) | 33% (partial) | paper, withdraw, keys |

### Backtesting

| Tool | Safety score | Missing inputs |
|---|---|---|
| [Backtesting.py](https://tradingagentstack.com/tool/backtesting-py/#safety) | 100% | none |
| [VectorBT](https://tradingagentstack.com/tool/vectorbt/#safety) | 90% | none |
| [QuantConnect / LEAN](https://tradingagentstack.com/tool/quantconnect-lean/#safety) | 60% | none |
| [NautilusTrader](https://tradingagentstack.com/tool/nautilustrader/#safety) | 47% (partial) | withdraw, keys |

### Broker APIs

| Tool | Safety score | Missing inputs |
|---|---|---|
| [Alpaca Trading API](https://tradingagentstack.com/tool/alpaca-trading-api/#safety) | 50% | none |
| [Interactive Brokers API](https://tradingagentstack.com/tool/interactive-brokers-api/#safety) | 41% (partial) | withdraw |
| [Tradier Brokerage API](https://tradingagentstack.com/tool/tradier-brokerage-api/#safety) | 41% (partial) | withdraw |
| [Schwab Trader API](https://tradingagentstack.com/tool/schwab-trader-api/#safety) | 17% (partial) | paper, withdraw, keys |

### Broker MCP servers

| Tool | Safety score | Missing inputs |
|---|---|---|
| [tastytrade MCP Server](https://tradingagentstack.com/tool/tastytrade-mcp-server/#safety) | 100% | none |
| [PrimeXBT MCP](https://tradingagentstack.com/tool/primexbt-mcp/#safety) | 90% | none |
| [eToro MCP Connectors](https://tradingagentstack.com/tool/etoro-mcp-connectors/#safety) | 90% | none |
| [Webull Cloud MCP Server](https://tradingagentstack.com/tool/webull-cloud-mcp-server/#safety) | 88% (partial) | paper |
| [TradeStation MCP](https://tradingagentstack.com/tool/tradestation-mcp/#safety) | 86% (partial) | paper, withdraw |
| [CCXT MCP Server](https://tradingagentstack.com/tool/ccxt-mcp-server/#safety) | 85% | none |
| [Axi MCP (MT5)](https://tradingagentstack.com/tool/axi-mcp-mt5/#safety) | 75% | none |
| [Interactive Brokers AI Integration (MCP)](https://tradingagentstack.com/tool/interactive-brokers-ai-integration-mcp/#safety) | 71% (partial) | paper |
| [Robinhood Trading MCP](https://tradingagentstack.com/tool/robinhood-trading-mcp/#safety) | 71% (partial) | paper |
| [Alpaca MCP Server](https://tradingagentstack.com/tool/alpaca-mcp-server/#safety) | 68% | none |
| [Longbridge MCP](https://tradingagentstack.com/tool/longbridge-mcp/#safety) | 68% | none |
| [cTrader AI Agent Connect (MCP)](https://tradingagentstack.com/tool/ctrader-ai-agent-connect-mcp/#safety) | 64% (partial) | paper, withdraw |
| [NinjaTrader MCP](https://tradingagentstack.com/tool/ninjatrader-mcp/#safety) | 58% | none |
| [moomoo MCP](https://tradingagentstack.com/tool/moomoo-mcp/#safety) | 58% | none |
| [Tradier MCP Server](https://tradingagentstack.com/tool/tradier-mcp-server/#safety) | 50% | none |
| [B2Trader MCP (B2PRIME)](https://tradingagentstack.com/tool/b2trader-mcp-b2prime/#safety) | 40% (partial) | paper, withdraw |
| [Public Hosted MCP Server](https://tradingagentstack.com/tool/public-hosted-mcp-server/#safety) | 28% (partial) | keys |

### Copy trading & strategy marketplaces

| Tool | Safety score | Missing inputs |
|---|---|---|
| [Darwinex Zero](https://tradingagentstack.com/tool/darwinex-zero/#safety) | 90% | none |
| [Bybit Copy Trading](https://tradingagentstack.com/tool/bybit-copy-trading/#safety) | 51% (partial) | paper |
| [eToro CopyTrader](https://tradingagentstack.com/tool/etoro-copytrader/#safety) | 51% (partial) | withdraw |
| [ZuluTrade](https://tradingagentstack.com/tool/zulutrade/#safety) | 44% (partial) | withdraw, keys |
| [MQL5 Signals](https://tradingagentstack.com/tool/mql5-signals/#safety) | 43% | none |
| [Collective2](https://tradingagentstack.com/tool/collective2/#safety) | 41% (partial) | withdraw |
| [Bitget Copy Trading](https://tradingagentstack.com/tool/bitget-copy-trading/#safety) | 29% (partial) | paper, withdraw |

### Exchanges & brokers for bots

| Tool | Safety score | Missing inputs |
|---|---|---|
| [Bitget](https://tradingagentstack.com/tool/bitget/#safety) | 85% | none |
| [Bybit](https://tradingagentstack.com/tool/bybit/#safety) | 85% | none |
| [Kraken](https://tradingagentstack.com/tool/kraken/#safety) | 85% | none |
| [OKX](https://tradingagentstack.com/tool/okx/#safety) | 85% | none |
| [Coinbase Advanced](https://tradingagentstack.com/tool/coinbase-advanced/#safety) | 75% | none |
| [Veranta MCP (formerly Avantis)](https://tradingagentstack.com/tool/veranta-mcp-formerly-avantis/#safety) | 75% | none |
| [GMX](https://tradingagentstack.com/tool/gmx/#safety) | 68% | none |
| [Lighter](https://tradingagentstack.com/tool/lighter/#safety) | 68% | none |
| [Paradex](https://tradingagentstack.com/tool/paradex/#safety) | 68% | none |
| [dYdX](https://tradingagentstack.com/tool/dydx/#safety) | 68% | none |
| [Pacifica](https://tradingagentstack.com/tool/pacifica/#safety) | 62% (partial) | withdraw |
| [Gemini](https://tradingagentstack.com/tool/gemini/#safety) | 60% | none |
| [Aster](https://tradingagentstack.com/tool/aster/#safety) | 58% | none |
| [Hyperliquid](https://tradingagentstack.com/tool/hyperliquid/#safety) | 50% | none |
| [Binance](https://tradingagentstack.com/tool/binance/#safety) | 49% | none |
| [Extended](https://tradingagentstack.com/tool/extended/#safety) | 43% | none |
| [edgeX](https://tradingagentstack.com/tool/edgex/#safety) | 29% (partial) | paper, withdraw |

### Market data APIs

| Tool | Safety score | Missing inputs |
|---|---|---|
| [OpenBB](https://tradingagentstack.com/tool/openbb/#safety) | 100% | none |
| [yfinance](https://tradingagentstack.com/tool/yfinance/#safety) | 100% | none |
| [Alpha Vantage API](https://tradingagentstack.com/tool/alpha-vantage-api/#safety) | 90% | none |
| [CoinBoss API](https://tradingagentstack.com/tool/coinboss-api/#safety) | 90% | none |
| [CrowdWisdomTrading Setups API](https://tradingagentstack.com/tool/crowdwisdomtrading-setups-api/#safety) | 90% | none |
| [Databento](https://tradingagentstack.com/tool/databento/#safety) | 90% | none |
| [Financial Datasets](https://tradingagentstack.com/tool/financial-datasets/#safety) | 90% | none |
| [Massive (Polygon) API](https://tradingagentstack.com/tool/massive-polygon-api/#safety) | 90% | none |
| [Poly Research & Robotics](https://tradingagentstack.com/tool/poly-research-robotics/#safety) | 90% | none |
| [SEC EDGAR APIs](https://tradingagentstack.com/tool/sec-edgar-apis/#safety) | 90% | none |
| [ThetaData](https://tradingagentstack.com/tool/thetadata/#safety) | 90% | none |

### Market data MCP servers

| Tool | Safety score | Missing inputs |
|---|---|---|
| [Alpha Vantage MCP](https://tradingagentstack.com/tool/alpha-vantage-mcp/#safety) | 100% | none |
| [Databento MCP servers (dbn-go)](https://tradingagentstack.com/tool/databento-mcp-servers-dbn-go/#safety) | 100% | none |
| [DexPaprika MCP](https://tradingagentstack.com/tool/dexpaprika-mcp/#safety) | 100% | none |
| [Massive (formerly Polygon) MCP](https://tradingagentstack.com/tool/massive-formerly-polygon-mcp/#safety) | 100% | none |
| [SiftingIO MCP](https://tradingagentstack.com/tool/siftingio-mcp/#safety) | 100% | none |
| [CryptoQuant MCP Server](https://tradingagentstack.com/tool/cryptoquant-mcp-server/#safety) | 90% | none |
| [DEBYKO MCP](https://tradingagentstack.com/tool/debyko-mcp/#safety) | 90% | none |
| [Lava MCP (A-share news heat)](https://tradingagentstack.com/tool/lava-mcp-a-share-news-heat/#safety) | 90% | none |
| [PredixLab MCP](https://tradingagentstack.com/tool/predixlab-mcp/#safety) | 90% | none |
| [Pyth Pro MCP Server](https://tradingagentstack.com/tool/pyth-pro-mcp-server/#safety) | 90% | none |
| [Redstone MCP](https://tradingagentstack.com/tool/redstone-mcp/#safety) | 90% | none |
| [Reslyce Flow MCP](https://tradingagentstack.com/tool/reslyce-flow-mcp/#safety) | 90% | none |
| [TradingView MCP Server](https://tradingagentstack.com/tool/tradingview-mcp-server/#safety) | 90% | none |

### On-chain & DeFi trading agents

| Tool | Safety score | Missing inputs |
|---|---|---|
| [Craic Hub Exchange](https://tradingagentstack.com/tool/craic-hub-exchange/#safety) | 80% | none |
| [1inch Swap API](https://tradingagentstack.com/tool/1inch-swap-api/#safety) | 71% (partial) | paper |
| [0x Swap API](https://tradingagentstack.com/tool/0x-swap-api/#safety) | 41% (partial) | paper |
| [Jupiter API](https://tradingagentstack.com/tool/jupiter-api/#safety) | 41% (partial) | paper |
| [Solana Agent Kit](https://tradingagentstack.com/tool/solana-agent-kit/#safety) | 35% | none |
| [BONKbot](https://tradingagentstack.com/tool/bonkbot/#safety) | 11% (partial) | keys |
| [Banana Gun](https://tradingagentstack.com/tool/banana-gun/#safety) | 11% (partial) | keys |
| [Maestro](https://tradingagentstack.com/tool/maestro/#safety) | 10% | none |
| [Trojan](https://tradingagentstack.com/tool/trojan/#safety) | 10% | none |

### Open-source trading bots

| Tool | Safety score | Missing inputs |
|---|---|---|
| [Vibe-Trading](https://tradingagentstack.com/tool/vibe-trading/#safety) | 62% (partial) | withdraw |
| [Freqtrade](https://tradingagentstack.com/tool/freqtrade/#safety) | 60% | none |
| [Hummingbot](https://tradingagentstack.com/tool/hummingbot/#safety) | 60% | none |
| [OctoBot](https://tradingagentstack.com/tool/octobot/#safety) | 60% | none |
| [Superalgos](https://tradingagentstack.com/tool/superalgos/#safety) | 60% | none |
| [Jesse](https://tradingagentstack.com/tool/jesse/#safety) | 53% (partial) | withdraw |
| [LumiBot](https://tradingagentstack.com/tool/lumibot/#safety) | 53% (partial) | withdraw |

### Prediction market APIs & agents

| Tool | Safety score | Missing inputs |
|---|---|---|
| [Limitless Exchange](https://tradingagentstack.com/tool/limitless-exchange/#safety) | 100% | none |
| [Prediction.Markets API](https://tradingagentstack.com/tool/prediction-markets-api/#safety) | 100% | none |
| [Manifold Markets API](https://tradingagentstack.com/tool/manifold-markets-api/#safety) | 90% | none |
| [Kalshi MCP Server (community)](https://tradingagentstack.com/tool/kalshi-mcp-server-community/#safety) | 85% | none |
| [Polymarket US API](https://tradingagentstack.com/tool/polymarket-us-api/#safety) | 67% (partial) | withdraw, keys |
| [Kalshi API](https://tradingagentstack.com/tool/kalshi-api/#safety) | 50% | none |
| [Polymarket Agents](https://tradingagentstack.com/tool/polymarket-agents/#safety) | 45% (partial) | paper |
| [DeskBot for Kalshi](https://tradingagentstack.com/tool/deskbot-for-kalshi/#safety) | 44% (partial) | withdraw, keys |
| [Polymarket API](https://tradingagentstack.com/tool/polymarket-api/#safety) | 30% | none |

### Risk, safety & paper trading

| Tool | Safety score | Missing inputs |
|---|---|---|
| [Agent Market Arena (AMA)](https://tradingagentstack.com/tool/agent-market-arena-ama/#safety) | 100% | none |
| [Guardrails AI](https://tradingagentstack.com/tool/guardrails-ai/#safety) | 100% | none |
| [Invariant Guardrails](https://tradingagentstack.com/tool/invariant-guardrails/#safety) | 100% | none |
| [NeMo Guardrails](https://tradingagentstack.com/tool/nemo-guardrails/#safety) | 100% | none |
| [PolicyGate Capital](https://tradingagentstack.com/tool/policygate-capital/#safety) | 100% | none |
| [Alpaca Paper Trading](https://tradingagentstack.com/tool/alpaca-paper-trading/#safety) | 90% | none |
| [Canopii Trust Index](https://tradingagentstack.com/tool/canopii-trust-index/#safety) | 90% | none |
| [IBKR Paper Trading Account](https://tradingagentstack.com/tool/ibkr-paper-trading-account/#safety) | 90% | none |
| [TradingView Paper Trading](https://tradingagentstack.com/tool/tradingview-paper-trading/#safety) | 90% | none |

### VPS & hosting for bots

| Tool | Safety score | Missing inputs |
|---|---|---|
| [AWS Lightsail](https://tradingagentstack.com/tool/aws-lightsail/#safety) | 90% | none |
| [Chocoping](https://tradingagentstack.com/tool/chocoping/#safety) | 90% | none |
| [DigitalOcean Droplets](https://tradingagentstack.com/tool/digitalocean-droplets/#safety) | 90% | none |
| [ForexVPS.net](https://tradingagentstack.com/tool/forexvps-net/#safety) | 90% | none |
| [Hetzner Cloud](https://tradingagentstack.com/tool/hetzner-cloud/#safety) | 90% | none |
| [QuantVPS](https://tradingagentstack.com/tool/quantvps/#safety) | 90% | none |

## Use it

- Download the JSON or CSV above, or read it live from `https://tradingagentstack.com/data/tools.json`.
- From an AI agent: the TradingAgentStack MCP server (`npx -y tradingagentstack-mcp`, or `https://tradingagentstack.com/api/mcp`) has `get_risk` and `get_incidents`.

## Corrections

Found a wrong fact? Open an issue with a link to the vendor's official docs, or use https://tradingagentstack.com/submit/. Facts without an official source aren't added.

## License

Data: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Credit "TradingAgentStack (tradingagentstack.com)". Not financial advice; verify with the vendor.
