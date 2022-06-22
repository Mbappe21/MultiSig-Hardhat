# Decentralized MultiSig

This is a Multiple Signature Wallet built with [Hardhat](https://hardhat.org/).

## Project Layout

This project allows you to create a DAO


1. `npm install`.

2. `npx hardhat compile`

3. `ganache-cli` or `npx hardhat node` to create a running blockchain.

4. `npx hardhat run scripts/deploy.js --network localhost` to deploy the MultiSig Wallet on this local blockchain.

5. `npx parcel app/index.html` to start the front-end

6. Connect one of the provided account to MetaMask.

7. Select 'Networks' tab, select 'Custom RPC' - then fill in:
- Network Name: you can name this anything you like
- RPC URL: `http://127.0.0.1:8545/`
- Chain ID: `31337`

Send some ETH to the contract, then submit a transaction that must be approved
by at least 2 owners (accounts provided on the running blockchain)
