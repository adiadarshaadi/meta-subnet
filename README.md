# Solidity ERC20 Token and Vault Contract 

## Overview

This repository contains two Solidity smart contracts: ERC20 and Vault. The ERC20 contract implements a basic ERC-20 token, while the Vault contract is designed to act as a simple vault for depositing and withdrawing ERC-20 tokens.

## ERC20 Token Contract

### Description

The ERC20 contract is a standard implementation of an ERC-20 token on the Ethereum blockchain. It includes basic functionalities such as token transfers, approvals, and allowance management. The token contract is named "SOLIDITY" (name) with the symbol "SOL" (ticker), and it has 18 decimal places.

### Functions

1. **transfer(address recipient, uint amount):** Transfers a specified amount of tokens from the sender to the recipient.

2. **approve(address spender, uint amount):** Allows a spender to spend a specified amount of tokens on behalf of the owner.

3. **transferFrom(address sender, address recipient, uint amount):** Transfers a specified amount of tokens from the sender to the recipient on behalf of the owner (if allowed).

4. **mint(uint amount):** Mints a specified amount of new tokens, increasing the total supply.

5. **burn(uint amount):** Burns a specified amount of tokens, decreasing the total supply.

### Events

- **Transfer(address indexed from, address indexed to, uint value):** Triggered on successful token transfers.

- **Approval(address indexed owner, address indexed spender, uint value):** Triggered on successful approvals.

## Vault Contract

### Description

The Vault contract is a basic implementation of a token vault, allowing users to deposit and withdraw ERC-20 tokens. The Vault contract is initialized with a specific ERC-20 token contract, and users can deposit and withdraw tokens based on the number of shares they own in the vault.

### Functions

1. **deposit(uint amount):** Allows users to deposit ERC-20 tokens into the vault, receiving shares in proportion to their deposit.

2. **withdraw(uint shares):** Allows users to withdraw ERC-20 tokens from the vault, burning the corresponding shares.

### Internal Functions

- **_mint(address to, uint shares):** Mints new shares to an address when they deposit tokens.

- **_burn(address from, uint shares):** Burns shares from an address when they withdraw tokens.

### Usage

1. Deploy the ERC20 token contract with the desired name, symbol, and decimals.

2. Deploy the Vault contract, passing the ERC20 token contract address as an argument.

3. Users can interact with the ERC20 token contract to transfer, mint, and burn tokens.

4. Users can deposit and withdraw ERC-20 tokens to and from the Vault contract, respectively.

## License

Both contracts are released under the MIT License. See the provided license files for more details.

## Author

Adarsh reddy P M

adi72597adi81816@gmail.com

