# **Solana Raydium Sniper**

The `Solana Raydium Sniper` is a high-performance bot designed to detect new token pools on Raydium and execute token buys and sells within the first block or first second after pool creation. It leverages advanced techniques, including `Jito block` engine and `Yellowstone gRPC` (via `Vibe Station`), for unparalleled transaction speed and efficiency, maximizing potential profits in DeFi trading.

## Key Features

- **🚀 Automated Pool Detection**: Monitors Raydium for new token pools and automatically initiates token purchases.
- **⚡ Sniping Within the First Block**: Executes transactions in the first block or second of pool creation using Yellowstone gRPC and Jito techniques.
- **🛠️ Jito Integration**: Utilizes Jito block engine for low-latency, high-speed transactions.
- **💡 Configurable Bot Settings**: Offers extensive customization via environment variables to suit diverse trading strategies.
- **🔄 Auto-Sell Functionality**: Includes automated selling with customizable take-profit and stop-loss settings.
- **🧠 Advanced Filters**: Filters tokens based on mint status, pool size, social checks, and other conditions.
- **📊 Real-Time Monitoring**: Tracks sniped tokens, monitors price changes, and executes optimized sell strategies.

## Environment Variables

Set up your `.env` file with the following parameters:

### General Settings

- `PRIVATE_KEY`: Your private wallet key.
- `RPC_ENDPOINT`: RPC endpoint for Solana network (e.g., https://staked.helius-rpc.com/?api-key=).
- `RPC_WEBSOCKET_ENDPOINT`: WebSocket endpoint for Solana network (e.g., wss://mainnet.helius-rpc.com/?api-key=).

### Buy Configuration

- `QUOTE_MINT`: Mint address of the token used for buying (e.g., WSOL).
- `QUOTE_AMOUNT`: Amount of token allocated for purchases.
- `MAX_BUY_RETRIES`: Maximum retry attempts for token buys.

### Sell Configuration

- `AUTO_SELL`: Enable or disable automated selling.
- `TAKE_PROFIT1` / TAKE_PROFIT2: Target profit levels.
- `STOP_LOSS`: Percentage for stop-loss execution.
- `PRICE_CHECK_INTERVAL`: Interval between price checks in milliseconds.
- `SELL_SLIPPAGE`: Allowed slippage percentage for sales.

### Filters

- `USE_SNIPE_LIST`: Use a predefined list of tokens for sniping.
- `CHECK_IF_MINT_IS_RENOUNCED`: Filter tokens based on mint renouncement.
- `MIN_POOL_SIZE / MAX_POOL_SIZE`: Limits for pool sizes eligible for sniping.

### Advanced Settings

- `JITO_MODE`: Enable Jito transaction mode.
- `BLOCKENGINE_URL`: URL of the Jito block engine server.
- `JITO_KEY`: API key for Jito transactions.
- `LOG_LEVEL`: Set the bot’s logging level (e.g., `info`).


## Usage Guide

#### 1. Install Dependencies
Clone the repository and install the necessary packages:

```
git clone https://github.com/Rabnail-SOL/Solana-Raydium-Sniper.git
cd Solana-Raydium-Sniper
npm install
```

#### 2. Set Environment Variables

Configure the `.env` file with your private key, RPC endpoints, and bot settings.

#### 3. Run the Bot
Start the sniping bot:
```
npm run buy
```

## **Super Raydium Sniper**
The bot is capable of sniping tokens within the `first block` or `first second` after pool creation. Using `Yellowstone gRPC` supported by `Vibe Station`, the bot achieves exceptional speed and reliability in detecting and executing trades.



## 👤 Contact Me

### Discord: [@knightworlds](https://discordapp.com/users/965772784653443215)

### Twitter: [@knightworlds127](https://twitter.com/knightworlds127)   

### Telegram: [@knightworlds](https://t.me/knightworlds)
