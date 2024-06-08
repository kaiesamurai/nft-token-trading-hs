# NFT Token Trading Platform

## Overview

This project is a decentralized NFT (Non-Fungible Token) trading platform built on the Secret Network. It offers cross-chain capabilities with networks such as Sepolia Ethereum, Scroll, and more, enabling secure and private trading of digital assets.

## Features

- **Secret Network Integration**: Utilizes Secret Network for privacy-preserving smart contracts.
- **Cross-Chain Compatibility**: Supports cross-chain transactions with Sepolia Ethereum and Scroll.
- **Secure Trading**: Ensures secure and private NFT transactions.
- **User-Friendly Interface**: Intuitive interface for easy trading and asset management.
- **Decentralized**: Fully decentralized platform with no central authority.

## Prerequisites

- [Node.js](https://nodejs.org/) (version 14.x or higher)
- [npm](https://www.npmjs.com/) (version 6.x or higher)
- [Docker](https://www.docker.com/) (for running local blockchain nodes)
- Secret Network CLI
- Ethereum wallet (e.g., MetaMask)

## Installation

### Clone the Repository

```bash
git clone https://github.com/yourusername/nft-token-trading.git
cd nft-token-trading
```

### Install Dependencies

```bash
npm install
```

### Configure Environment Variables

Create a `.env` file in the root directory and add the following variables:

```bash
SECRET_NETWORK_RPC_URL=<your-secret-network-rpc-url>
SEPOLIA_ETH_RPC_URL=<your-sepolia-eth-rpc-url>
SCROLL_RPC_URL=<your-scroll-rpc-url>
PRIVATE_KEY=<your-private-key>
```

### Running the Project

#### Start Local Blockchain Nodes (Optional)

If you need to run local nodes for testing:

1. **Secret Network**:
    ```bash
    docker run -it --rm -p 26657:26657 -p 1317:1317 -p 5000:5000 \
    --name secret-node enigmampc/secret-network-local:latest
    ```

2. **Sepolia Ethereum** and **Scroll** nodes can be started similarly using their respective Docker images.

#### Start the Application

```bash
npm start
```

The application will be available at `http://localhost:3000`.

## Usage

1. **Connect Wallet**: Use MetaMask or any supported wallet to connect to the platform.
2. **Mint NFT**: Navigate to the minting section to create your own NFTs.
3. **Trade NFT**: Use the marketplace to list your NFTs for sale or purchase available NFTs.
4. **Cross-Chain Transactions**: Utilize the cross-chain functionality to trade NFTs across different networks.

## Project Structure

- **src/**: Contains the source code for the application.
  - **components/**: React components for the UI.
  - **contracts/**: Smart contracts for Secret Network and other blockchains.
  - **services/**: Services for interacting with blockchain nodes.
  - **utils/**: Utility functions and helpers.
- **public/**: Public assets and static files.
- **.env**: Environment variables.

## Contributing

We welcome contributions from the community! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch-name`.
3. Make your changes and commit them: `git commit -m 'Add new feature'`.
4. Push to the branch: `git push origin feature-branch-name`.
5. Create a pull request.


Thank you for using our NFT Token Trading Platform! We hope you enjoy the seamless and secure trading experience.