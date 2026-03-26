# HederaOracle MCP Server

**9 DeFi risk & compliance intelligence tools for the Hedera ecosystem.**

Enterprise-grade network with Google, IBM, Boeing on the Governing Council. HTS token key analysis for institutional risk assessment.

## Live Endpoint

```
https://tooloracle.io/hedera/mcp/
```

No API key required. MIT licensed.

## Quick Setup

```json
{
  "mcpServers": {
    "hederaoracle": {
      "url": "https://tooloracle.io/hedera/mcp/"
    }
  }
}
```

## Tools (9)

| Tool | Description | Data Source |
|------|-------------|------------|
| `hbar_overview` | Hedera ecosystem: HBAR price, TVL, supply, Governing Council, protocols | CoinGecko + DeFiLlama + Mirror Node |
| `hbar_account_info` | Account balance, key type, token holdings | Hedera Mirror Node |
| `hbar_token_info` | HTS token risk analysis: admin/freeze/wipe/supply/pause keys with risk scoring | Hedera Mirror Node |
| `hbar_protocol_health` | Protocol health: TVL, audits, risk grade (SaucerSwap, Stader, HeliSwap...) | DeFiLlama |
| `hbar_defi_yields` | Compare DeFi yields across Hedera protocols | DeFiLlama Yields |
| `hbar_protocol_list` | All Hedera DeFi protocols ranked by TVL | DeFiLlama |
| `hbar_stablecoin_risk` | Stablecoin supply and risk on Hedera | DeFiLlama |
| `hbar_network_stats` | Network stats: supply, nodes, consensus info | Hedera Mirror Node |
| `hbar_transactions` | Recent transactions for any Hedera account | Hedera Mirror Node |

## Key Feature: HTS Token Key Analysis

Hedera Token Service (HTS) tokens have granular key permissions. `hbar_token_info` checks all keys:

- **Admin Key** — Can modify token properties
- **Freeze Key** — Can freeze token transfers
- **Wipe Key** — Can wipe token balances
- **Supply Key** — Can mint/burn tokens
- **Pause Key** — Can pause all operations

Each key impacts the risk score. Tokens with fewer keys = lower risk.

## Data Sources

- **Hedera Mirror Node** (mainnet.mirrornode.hedera.com) — Accounts, tokens, transactions, network
- **DeFiLlama** — TVL, yields, stablecoins, DEX volumes
- **CoinGecko** — Prices, market data

## Links

- **Live endpoint**: https://tooloracle.io/hedera/mcp/
- **Health check**: https://tooloracle.io/hedera/health
- **Builder**: [FeedOracle Technologies](https://feedoracle.io) — EU-based compliance infrastructure
- **Marketplace**: [ToolOracle](https://tooloracle.io)
- **License**: MIT
