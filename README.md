# Flashbots MEV Searcher Guide

This guide helps you build a Miner Extractable Value (MEV) searcher using Flashbots.

## Setup

- Install Node.js, npm.
- Set `QUICKNODE_RPC_URL`, `QUICKNODE_WS_URL`, `PRIVATE_KEY` in `.env`.
- Install npm packages: `@nomicfoundation/hardhat-toolbox`, `dotenv`, `@flashbots/ethers-provider-bundle`, `ethers`, `hardhat`.

## Components

- `FakeNFT.sol`: A simple ERC721 contract.
- `hardhat.config.js`: Hardhat configuration.
- `deploy.js`: Script for contract deployment and transaction bundling.

## Usage

1. Clone the repository.
2. Install dependencies: `npm install`.
3. Compile the contract: `npx hardhat compile`.
4. Run the script: `node deploy.js`.
5. Run Flashbots script: `npx hardhat run scripts/flashbots.js --network sepolia`.

**Note**: Secure your `.env` file and private key. Replace `sepolia` with your network. Audit contracts before mainnet deployment.
