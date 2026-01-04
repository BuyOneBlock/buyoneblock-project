# Buy One Block — Smart Contract Integration Guide

## 1. Overview
This guide explains how to integrate the Buy One Block smart contract into any Web3 application, wallet, or backend service. It includes ABI usage, contract address, network details, and sample code for developers.

---

## 2. Contract Details
- **Network**: BNB Smart Chain (Mainnet)
- **Contract Address**: `0x6Cc08F61612C14098F9B230A474EE34d9584D56e`
- **Token Symbol**: `1BONEBU`
- **Decimals**: `18`
- **Total Supply**: `320,000,000`
- **Standard**: BEP‑20 (ERC‑20 compatible)
- **ABI File**: `abi.json`

---

## 3. ABI Usage
```js
// ES Module
import abi from './abi.json';

// CommonJS
const abi = require('./abi.json');

---
## 4. Web3.js Integration**

import Web3 from 'web3';
import abi from './abi.json';

const provider = 'https://bsc-dataseed.binance.org/';
const web3 = new Web3(provider);

const contractAddress = '0x6Cc08F61612C14098F9B230A474EE34d9584D56e';
const contract = new web3.eth.Contract(abi, contractAddress);

// Example: Read token name
contract.methods.name().call().then(console.log);

---
5. Ethers.js Integration

import { ethers } from 'ethers';
import abi from './abi.json';

const provider = new ethers.JsonRpcProvider('https://bsc-dataseed.binance.org/');
const contractAddress = '0x6Cc08F61612C14098F9B230A474EE34d9584D56e';

const contract = new ethers.Contract(contractAddress, abi, provider);

// Example: Read token name
const name = await contract.name();
console.log(name);

---
6. Wallet Integration (MetaMask / SafePal)
Add Token Manually

Token Contract: 0x6Cc08F61612C14098F9B230A474EE34d9584D56e

Symbol: 1BONEBU

Decimals: 18

Notes

Ensure the wallet is set to BNB Smart Chain

Use the ABI from abi.json for contract interactions

---
7. Security Notes
Always verify the contract address before integration

Never hardcode private keys

Use HTTPS RPC endpoints

Validate user input before calling contract functions

---
8. Developer Resources
RPC Endpoint: https://bsc-dataseed.binance.org/

ABI File: abi.json

Contract Address: 0x6Cc08F61612C14098F9B230A474EE34d9584D56e

9. Support
For technical integration or partnership inquiries: buyoneblock@buy_one_block.com
