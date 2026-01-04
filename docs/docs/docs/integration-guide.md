# Buy One Block — Smart Contract Integration Guide

## 1. Overview

This guide explains how to integrate the Buy One Block smart contract into any Web3 application, wallet, or backend service.  
It includes ABI usage, contract address, network details, and sample code for developers.

---

## 2. Contract Details

- **Network**: BNB Smart Chain (Mainnet)  
- **Contract Address**: `0x6Cc08F61612C14098F9B230A474EE34d9584D56e`  
- **Token Symbol**: `1BONEBU`  
- **Decimals**: `18`  
- **Total Supply**: `320,000,000`  
- **Standard**: BEP-20 (ERC-20 compatible)  
- **ABI File**: [`abi.json`](./abi.json)

---

## 3. ABI Usage

To interact with the contract, import the ABI from `abi.json`:

```js
import abi from './abi.json';

const abi = require('./abi.json');


import Web3 from 'web3';
import abi from './abi.json';

const web3 = new Web3('https://bsc-dataseed.binance.org/');
const contractAddress = '0x6Cc08F61612C14098F9B230A474EE34d9584D56e';
const contract = new web3.eth.Contract(abi, contractAddress);

// Example: Read token name
contract.methods.name().call().then(console.log);

import { ethers } from 'ethers';
import abi from './abi.json';

const provider = new ethers.JsonRpcProvider('https://bsc-dataseed.binance.org/');
const contractAddress = '0x6Cc08F61612C14098F9B230A474EE34d9584D56e';
const contract = new ethers.Contract(contractAddress, abi, provider);

// Example: Read token name
const name = await contract.name();
console.log(name);


Wallet Integration (MetaMask / SafePal)
To add the token manually:

Token Contract: 0x6Cc08F61612C14098F9B230A474EE34d9584D56e

Symbol: 1BONEBU

Decimals: 18

To interact with the contract:

Use the ABI from abi.json

Connect via window.ethereum or SafePal SDK

Ensure the wallet is on BNB Smart Chain
