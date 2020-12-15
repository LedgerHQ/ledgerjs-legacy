> **IMPORTANT: this package is deprecated due to the fact we had to move away from U2F. Contributions are welcome to make it running in WebUSB!**

---

# Ledger DApp Ethereum starter kit

Welcome to Ledger DApp starter kit, web app backed by Ethereum smart contract. Out of the box support of Ledger devices and MetaMask.

**bootstrap a project with:**

```
yarn create dapp new-project-name
```

OR

```
npm i -g create-dapp
create-dapp new-project-name
```

![](https://user-images.githubusercontent.com/211411/35970466-b4985312-0cca-11e8-9baf-33e60ec9ac70.gif)

## Pre-requisite documentation to read

* React: https://reactjs.org
* Solidity: https://solidity.readthedocs.io
* web3.js: https://github.com/ethereum/web3.js
* truffle-contract: https://github.com/trufflesuite/truffle-contract

## Pre-requisite tools to install

```
npm install -g truffle ganache-cli
```

## Develop

Run a development Ethereum network:

```
ganache-cli --networkId 1337
```

> Alternatively you can run on Ethereum testnet.

Run the truffle tool, to generate and compile the contracts. **NB: the truffle project lives under src/dapp**

```
cd src/dapp
truffle compile
truffle deploy --network development
```

> Adapt the deploy based on your need. Read truffle documentation for more information.

Run the web app:

```
npm start
```

> Read create-react-app documentation for more information.
