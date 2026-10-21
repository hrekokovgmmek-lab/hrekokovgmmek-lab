# Artem Vartanov

**Solana developer — low-latency trading systems and on-chain analytics.**

I build trading bots and monitoring tools for Solana and back every number with measurements. My own system,
memesniper, has made **1,263 live trades** on Solana mainnet: **under 1 s** from signal to a sent transaction, a
**3.3 GB** market dataset and **25+ preregistered experiments**.

### What I build

- **Trading bots** — sniping, target / stop / time-based exits, manual-control terminals
- **Monitoring** — wallets (copy-trading signals), new tokens and migrations, with Telegram alerts and risk filters
- **On-chain data** — collection pipelines, datasets, dashboards, investigations (bundles, sniper wallets)
- **Audits** — backtests and bots: I find where the numbers disagree with reality

### Projects

| Project | What it shows |
|---|---|
| [pumpfun-migration-alerts](https://github.com/hrekokovgmmek-lab/pumpfun-migration-alerts) | Real-time pump.fun → PumpSwap migration alerts with on-chain risk flags: PDA pool derivation, forward-compatible account decoding, a single-socket feed with backoff, rate-limited RPC, 21 tests |
| [solana-wallet-tracker](https://github.com/hrekokovgmmek-lab/solana-wallet-tracker) | Real-time buys and sells of any Solana wallet, read from balance changes so it works on every DEX: rent and wrapped-SOL accounting, a slot heartbeat, backpressure, a top-holders mode, 19 tests (two on real mainnet transactions) |
| [pumpswap-fee-decoder](https://github.com/hrekokovgmmek-lab/pumpswap-fee-decoder) | Where the money in a PumpSwap trade goes, to the lamport: events decoded with the program's own on-chain IDL, fees checked against the pool vault (found fees held in the pool for later), priority fees, tips and bot fees, the live fee-tier table |
| [honest-backtest](https://github.com/hrekokovgmmek-lab/honest-backtest) | An honesty report for any backtest or trade log: day-resampled bootstrap next to the naive interval, one-day and tail dependence, deflated Sharpe, power, break-even, replay red flags, and preregistration that freezes code and data by sha256 |
| [solana-fund-tracer](https://github.com/hrekokovgmmek-lab/solana-fund-tracer) | Follow money on Solana from a wallet back to its source and forward to exchange deposit addresses: walks that stop at exchanges, busy addresses and loops, deposit detection by sweeps into labelled hot wallets, memo-hidden payers, a resumable full-history ledger; Python standard library only, 22 tests |
| [research-ledger](https://github.com/hrekokovgmmek-lab/research-ledger) | An append-only log of results and decisions, and preregistrations that freeze code and data by sha256 and let the outcome be read once: early, edited and repeated reads are refused, corrections never overwrite; Python standard library only, 20 tests |


### Stack

TypeScript · Node.js · Python · @solana/web3.js · WebSocket / JSON-RPC · Token-2022 · pump.fun / PumpSwap ·
Electron · node:test

### How I work

- No profit promises — I am responsible for the bot doing what it was designed to do
- Your keys stay with you: bots run with your wallet on your machine or server
- No wash-trading volume bots, drainers or bundlers for rug launches

### Contact

Telegram — [@artemvartanov](https://t.me/artemvartanov) · Russian and English (B1–B2) · UTC+3
