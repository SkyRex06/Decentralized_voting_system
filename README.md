# Decentralized Voting System

## Introduction

The Decentralized Voting System is a blockchain-based voting platform designed to ensure security, transparency, and tamper-proof elections. By eliminating central authorities, it allows votes to be recorded immutably and verified by all participants, reducing the risk of fraud and manipulation.

## Table of Contents

-   [Introduction](#introduction)
-   [Features](#features)
-   [Project Structure](#project-structure)
-   [Getting Started](#getting-started)
    -   [Prerequisites](#prerequisites)
    -   [Installation](#installation)
    -   [Running the Application](#running-the-application)
-   [Usage](#usage)
-   [Technologies Used](#technologies-used)
-   [Contributing](#contributing)
-   [License](#license)

## Features

- **Blockchain Security:** Immutable and tamper-proof voting records.
- **Transparency:** Votes can be verified without revealing voter identity.
- **Decentralization:** No single point of control, ensuring fairness.
- **Anonymity:** Voter privacy is maintained while ensuring authenticity.
- **Real-time Results:** Instant and verifiable vote counting

## How It Works
-  **User Registration**: Users sign up and verify their identity using a blockchain wallet.
-  **Casting Votes:** Users cast votes through a smart contract, ensuring security.
-  **Verification:** Votes are stored on the blockchain, making them immutable.
-  **Result Calculation:** Real-time tallying without manipulation

## Project Structure
### Prerequisites

-   Node.js (LTS version recommended)
-   npm (Node Package Manager, comes with Node.js)
-   Truffle (`npm install -g truffle`)
-   Ganache (Ganache UI recommended; `npm install -g ganache`)
-   MetaMask (Browser extension for interacting with Ethereum)

### Installation

1.  Clone the repository:

    ```bash
    git clone [repository URL]
    cd decentralized-voting-system
    ```

2.  Install dependencies:

    ```bash
    npm install
    ```

### Running the Application

1.  Start Ganache (Ganache UI is recommended).

2.  Compile the smart contract:

    ```bash
    truffle compile
    ```

3.  Deploy the contract to Ganache:

    ```bash
    truffle migrate
    ```

4.  Copy the contract address and ABI from the deployment output.  You'll find the ABI in `build/contracts/Voting.json`.

5.  In the `frontend/script.js` file, replace `YOUR_CONTRACT_ADDRESS` and `YOUR_CONTRACT_ABI` placeholders with your actual contract address and ABI.

6.  Open `frontend/index.html` in your browser.

7.  Connect MetaMask to your Ganache network.

## Usage

1.  Open the `index.html` file in your browser.
2.  Connect MetaMask to your Ganache network and select an account.
3.  The candidate names should be displayed.
4.  Implement candidate selection in your frontend (e.g., radio buttons, dropdown).
5.  Click the "Vote" button to cast your vote.  MetaMask will prompt you to confirm the transaction.

## Technologies Used

-   **Solidity:** Smart contract programming language.
-   **JavaScript:** Frontend logic and interaction with the smart contract.
-   **Web3.js:** JavaScript library for interacting with the Ethereum blockchain.
-   **Truffle:** Development framework for Ethereum dApps.
-   **Ganache:** Local Ethereum blockchain for development.
-   **MetaMask:** Browser extension for managing Ethereum accounts and signing transactions.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

