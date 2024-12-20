# Onchain Trading Bot

This project is a Telegram bot designed for on-chain trading. Users can check their balance, deposit and withdraw ETH, trade (buy/sell) assets, and export their private keys securely. The bot is built with the Grammy framework, Coinbase SDK, and integrates with a database for wallet management.

---

## Features

1. **User-Friendly Interface**:
   - Inline menu with options for balance checking, deposits, withdrawals, and trades.
   - Interactive prompts for a seamless user experience.

2. **Secure Wallet Management**:
   - Uses encryption to store user wallet data securely.
   - Wallets are created and managed on the Coinbase SDK.

3. **Flexible Trading**:
   - Buy and sell assets using ETH as the base currency.
   - Validates transactions and balances before execution.

4. **ETH Deposit and Withdrawal**:
   - Easily deposit ETH to your wallet.
   - Withdraw ETH to any address or ENS name.

5. **Advanced Capabilities**:
   - Export private keys for backup.
   - Pin important messages in chat for quick reference.

---

## Prerequisites

- Node.js (>=14.0.0)
- npm or yarn
- Telegram bot token
- Coinbase API key and secret
- A 32-byte encryption key (in hexadecimal)

---

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/onchain-trading-bot.git
   cd onchain-trading-bot
   ```

2. Install the required dependencies:

   ```bash
   npm install
   ```

3. Set up environment variables. Create a `.env` file in the root directory and include the following:

   ```env
   TELEGRAM_BOT_TOKEN=your_telegram_bot_token
   COINBASE_API_KEY_NAME=your_coinbase_api_key_name
   COINBASE_API_KEY_SECRET=your_coinbase_api_key_secret
   ENCRYPTION_KEY=your_32_byte_encryption_key_in_hex
   ```

---

## Usage

1. Start the bot:

   ```bash
   node bot.js
   ```

2. Add the bot to a Telegram chat and use `/start` to begin interacting.

3. Select options from the menu:
   - **Check Balance**: Displays the current balance of the wallet.
   - **Deposit ETH**: Provides the wallet address for ETH deposits.
   - **Withdraw ETH**: Guides the user through the withdrawal process.
   - **Buy/Sell**: Facilitates asset trading.
   - **Export Key**: Exports the private key securely.

---

## Security

- Wallet data is encrypted using AES-256-CBC.
- Private keys are only displayed on user request and should be stored securely by the user.

---

## Dependencies

- [Grammy](https://grammy.dev/) - Telegram bot framework
- [Coinbase SDK](https://github.com/coinbase/coinbase-node) - Wallet and trading operations
- [Replit Database](https://www.npmjs.com/package/@replit/database) - Lightweight database
- [Web3.js](https://web3js.readthedocs.io/) - Ethereum blockchain interaction
- [Decimal.js](https://mikemcl.github.io/decimal.js/) - Precision arithmetic
- [crypto](https://nodejs.org/api/crypto.html) - Encryption utilities

---

## License

This project is licensed under the MIT License.
