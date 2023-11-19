# Building-on-Avalanche---ETH-AVAX

## Overview
DegenToken is an ERC-20 token contract written in Solidity. It allows users to buy predefined items using the token and includes basic functionalities like minting, burning, and transferring tokens.

## Features
- Minting: The contract owner can mint additional tokens.
- Burning: Users can burn a specified amount of their tokens.
- Buying Items: Users can buy predefined items using their tokens.

## Items
The contract comes with default items during deployment:
1. Tshirt (Price: 20 tokens) - Index: 0
2. Pants (Price: 50 tokens) - Index: 1
3. Underwear (Price: 100 tokens) - Index: 2

## Functions
- `addItem(string memory name, uint256 price)`: Add a new item to the contract.
- `getItem(uint256 index) public view returns (string memory name, uint256 price)`: Get details of an item by index.
- `mint(uint256 amount)`: Mint additional tokens (onlyOwner).
- `burn(uint256 amount)`: Burn a specified amount of tokens.
- `buyItem(uint256 itemIndex)`: Buy an item by index, burning the required tokens.
