# Decentralized Voting System

This project implements a decentralized voting system using Solidity smart contracts, a JavaScript frontend, and Web3.js for blockchain interaction.  It's designed as a prototype for a FOSS hackathon.

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

## Introduction

This decentralized voting system aims to provide a transparent and secure platform for casting votes. By leveraging blockchain technology, it ensures that votes are immutable and tamper-proof. This prototype focuses on core voting functionality and serves as a foundation for future enhancements.

## Features

-   **Candidate Registration (Hardcoded for MVP):** Initial candidates are defined within the smart contract's constructor for simplicity in this prototype.
-   **Secure Voting:** Voters can cast their vote for a single candidate. Double voting is prevented.
-   **Transparent Vote Counting:** Vote counts for each candidate can be retrieved and viewed.
-   **Decentralized:** The voting process is managed by a smart contract on the Ethereum blockchain (or a compatible network).

## Project Structure
## Getting Started

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

## License

[Choose a license - e.g., MIT]
