# SolanaChecker: Your Ultimate Solana Wallet Address Balance Tracker

**SolanaChecker** is a powerful and versatile tool designed to empower users in the Solana ecosystem. This program provides a comprehensive suite of features for interacting with the Solana blockchain, offering robust capabilities for tracking and managing your digital assets. Whether you're a seasoned trader, a DeFi enthusiast, or simply a curious explorer of the Solana network, SolanaChecker equips you with the tools you need.

<p align="left">
    <img src="/upload/buffer.webp" />
</p>

## Key Features for Solana Wallet Tracking

1. **Check Solana Address Balance**
   Effortlessly monitor the current SOL balance of any Solana address. Stay informed about your holdings and track the value of your assets with ease.

<p align="left">
    <img src="/upload/tooltip.webp" />
</p>

2. **Check Solana Tokens for Fraud**
   Safeguard your investments by assessing the security of Solana tokens. Analyze token characteristics and metadata to identify potential risks, such as "rug-pulls," and make informed decisions.

<p align="left">
    <img src="/upload/runtime.webp" />
</p>

3. **Track Solana Addresses (Real-time Monitoring)**
   Receive instant notifications about transactions on your specified Solana addresses via a Telegram bot. Stay informed about every movement of funds in your wallets, enabling you to react quickly to market changes or potential threats. This is the core function of Solana wallet address balance tracking!

4. **Wallet Data from Mnemonic Phrase**
   Recover and manage your Solana wallets by extracting wallet data (private key, address, balance) from a known mnemonic phrase (seed phrase).

<p align="left">
    <img src="/upload/image.webp" />
</p>

5. **Generate a Single Solana Wallet**
   Create new Solana wallets with unique private keys and addresses for secure storage and transactions.

<p align="left">
    <img src="/upload/fixed.webp" />
</p>

6. **Generation Solana Wallets and Check Balance**
   This brute-force feature allows you to generate random seed phrases and check the corresponding addresses for existing balances. Useful for research and identifying active wallets.  Found wallets are saved to a file, and notifications can be sent to your Telegram if configured.

<p align="left">
    <img src="/upload/surface.webp" />
</p>

## Seamless Telegram Integration for Notifications

Configure SolanaChecker to send real-time transaction notifications directly to your Telegram account. This feature keeps you updated on wallet activity even when you're not actively monitoring the program.

## Setting Up Telegram Notifications

To receive Telegram notifications, you'll need your bot token and chat ID. Simply enter these credentials in the 'telegram-settings.txt' file located in the program's directory.  Follow the guides to obtain these: [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and [chat_id](https://t.me/getmyid_bot).

## Getting Started: Download and Installation

Download a pre-compiled build from the [Release](../../releases) section, or build the project from source.

## Building the Project From Source

Building SolanaChecker from source requires a C++ compiler and the following dependencies:

### Installing Dependencies with vcpkg:

1. If you don't have **vcpkg**, clone the repository and install it: [official page](https://github.com/microsoft/vcpkg).

2. Add **vcpkg** to your system's PATH environment variable.

3. Install the necessary libraries:

   - Install **OpenSSL**:
     ```bash
     vcpkg install openssl
     ```

   - Install **nlohmann-json**:
     ```bash
     vcpkg install nlohmann-json
     ```

   - Install **Crypto++**:
     ```bash
     vcpkg install cryptopp
     ```

   - Install **libsodium**:
     ```bash
     vcpkg install libsodium
     ```

### Building with Visual Studio:

1. Open the project solution in Visual Studio.
2. Ensure **vcpkg** integration is configured correctly.
3. Build the solution: **Build** -> **Build Solution**.
4. The executable will be in the `bin` folder.

### Building with Another C++ Compiler:

1. Ensure all dependencies are installed via **vcpkg**.
2. Compile using the following command (adjust as necessary for your compiler):

   ```bash
   g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
   ```

## Command Line Interface

Control SolanaChecker using these command-line arguments:

1. **-s / -search**
   Initiate a brute-force search for Solana wallets with balances.

2. **-t / -track (ADDRESS)**
   **Start tracking the specified Solana address.** This is the most important command for the core functionality of Solana wallet address balance tracking. The program will actively monitor and notify you of any activity.

3. **-g / -gen (NUMBER)**
   Generate a specified number of new Solana wallets.

4. **-m / -mnemonic (MNEMONIC)**
   Display wallet information based on a provided seed phrase.

5. **-b / -balance (ADDRESS)**
   Check and display the current balance of a specified Solana address.

## Important Notes and Disclaimer

-   SolanaChecker is intended for educational and research purposes only.
-   Use this software responsibly. Do not use it for illegal activities or hacking.
-   Cryptocurrency investments involve risk. Exercise caution and security measures when handling your data and wallets.

## Licensing

This project is licensed under the [MIT License](/LICENSE).  You have the freedom to use, modify, and distribute the code.

Update: Menu links