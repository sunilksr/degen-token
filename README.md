# DegenToken 

## Overview

This repository contains the source code for the `DegenToken` smart contract, which is an ERC-20 token deployed on the Ethereum blockchain. The contract is named "Degen" and has the symbol "DGN." It includes additional functionalities such as minting, burning, transferring tokens, and redeeming watches.

## Smart Contract Features

### ERC-20 Compliance

The smart contract follows the ERC-20 standard, providing basic functionalities for managing and transferring tokens.

### Ownership

The contract extends the `Ownable` contract from OpenZeppelin, ensuring that certain functions can only be executed by the owner of the contract.

### Burning Tokens

Token holders can burn their tokens, reducing their own balance. This is done through the `burnTokens` function.

### Minting Tokens

The owner of the contract can mint additional tokens and allocate them to a specified address using the `mintTokens` function.

### Transferring Tokens

Token holders can transfer their tokens to other addresses using the `transferTokens` function.

### Watch Redemption

Token holders can redeem watches using the `redeemWatch` function. Each watch has a name, rate, and quantity associated with it. The redemption process involves burning a specific number of tokens based on the watch's rate and decrementing the watch's quantity.

## Watches

The contract maintains a mapping of watches, where each watch is represented by a unique name. Watches have associated rates (token cost per watch) and quantities.

### Example Watches

1. **Rolex**
   - Rate: 100 tokens
   - Quantity: 10

2. **Casio**
   - Rate: 50 tokens
   - Quantity: 20

3. **Omega**
   - Rate: 40 tokens
   - Quantity: 15

4. **Seiko**
   - Rate: 30 tokens
   - Quantity: 25

## Functions

- `mintTokens`: Only the owner can mint additional tokens and allocate them to a specified address.
- `burnTokens`: Token holders can burn their own tokens, reducing their balance.
- `transferTokens`: Token holders can transfer tokens to other addresses.
- `redeemWatch`: Token holders can redeem watches by providing the watch name and quantity, burning the required tokens.

## Author

Sunil ks

## License

This smart contract is released under the MIT License. See the `LICENSE` file for more details.
