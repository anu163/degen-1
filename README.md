# DegenToken Smart Contract

This repository contains a Solidity smart contract named DegenToken. DegenToken is an ERC-20 token with additional functionality, including minting, transferring, burning tokens, and redeeming specific tokens. The contract also provides a function to retrieve a predefined list of tokens and their values.

## Contract Details

- **Name**: DegenToken
- **Symbol**: DGN

## Features

- Mint new tokens: The contract owner can mint new Degen tokens and allocate them to specific addresses.

- Transfer tokens: Token holders can transfer their tokens to other addresses using the `transferTokens` function.

- Burn tokens: Token holders can burn (destroy) a specified number of tokens using the `burnTokens` function.

- Redeem tokens: Token holders can redeem their tokens for predefined items listed with corresponding values. This is done through the `redeemTokens` function.

## Usage

1. Deploy the DegenToken contract to an Ethereum-compatible blockchain.

2. As the contract owner, mint initial tokens using the `mint` function.

3. Users can transfer their tokens using the `transferTokens` function.

4. Users can burn their tokens using the `burnTokens` function.

5. Users can redeem tokens for predefined items using the `redeemTokens` function. Provide the choice number (1-5) as an argument to redeem a specific item.

## Important

This contract is provided as a sample and should not be used in production without thorough testing and auditing.

Ensure you understand the contract's functionality and implications before interacting with it.

## Example

```solidity
// Deploy DegenToken contract

// Mint initial tokens to an address
contract.mint(userAddress, amount);

// Transfer tokens from one address to another
contract.transferTokens(toAddress, amount);

// Burn tokens to reduce supply
contract.burnTokens(amount);

// Redeem tokens for a predefined item
contract.redeemTokens(choice);

