
BSC/EVM Mempool Monitoring Frontrun Bot for Pancakeswap (Delta Edition)

This is a Pancakeswap frontrunning bot targeting EVM-compatible networks, including Binance Smart Chain (BSC), Ethereum (ETH), Avalanche (AVAX), Polygon (MATIC), Fantom (FTM), Cronos (CRO), Harmony (ONE), Milkomeda (MilkADA), Moonforce, etc. Capable of replacing wallet addresses within detected txs.

This project is provided for research and educational purposes only. Use responsibly and in accordance with applicable laws and platform terms.

## Features

- ⚡ Lightning-fast mempool sniping
- 🥞 PancakeSwap V2 support
- 💸 Automatic buy/sell with customizable profit targets
- 🔒 Secure private key management (never leaves your machine)
- 💰 Designed to maximize profit during new token launches and liquidity events
- 🛡️ Anti-rugpull, anti-honeypot checks (optional)
- 📈 Real-time monitorings
- 👛 Wallet-replacing capability
- Multi-chain EVM support
- Mempool transaction decoding (via `abi-decoder`)
- Web3-based interaction with nodes (`web3`)
- Configurable runtime parameters (see `src/env.js` and `src/constants.js`)

## Requirements


- Node.js and npm (LTS recommended, Linux recommended)
- Windows users: Visual Studio C++ Build Tools (only if native modules are required)

## Getting Started

1. Install dependencies:
   
   ```bash
   npm install
   ```

2. Configure environment:
   - Update `env.js` with your RPC endpoints and credentials (e.g., private key).
   - Adjust `constants.js` for chain IDs, contract addresses, gas settings, and other operational parameters.

3. Run the bot:

   ```bash
   node frontrun.js
   ```

## Configuration

- `env.js`: Sensitive runtime values such as RPC URLs and private keys. Keep this file secure and never commit secrets.
- `constants.js`: Network and application constants (e.g., router addresses, WETH/WBNB addresses, gas multipliers).

Feel free to reach out for implementation assistance or integration support.

## Security Notes

- Never commit private keys or credentials.
- Prefer environment variables or a secrets manager in production.
- Use dedicated wallets and risk controls when operating on mainnet.

## Legal Disclaimer

This software is provided “as is,” without warranty of any kind. You are solely responsible for compliance with laws, exchange/DEX terms, and all risks (including financial loss) arising from use of this software.

This tool is for educational purposes only. Use at your own risk. The author is not responsible for any financial losses or legal issues.

## FAQ

**Q: Is this safe?**
A: The bot never uploads your private key. All transactions are signed locally.

**Q: Is this legal?**
A: This is for educational and research purposes only. Use at your own risk.

**Q: How much can I expect to make in a day?**
A: I managed to make 0.5 BNB in 1 day, however your results maybe different. You may make more or less than when I first tested this tool.

## Binaries

Precompiled binaries are not provided in this repository. Build and run from source as described above.
