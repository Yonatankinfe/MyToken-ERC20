# MyToken-ERC20
A simple implementation of an ERC-20 token standard in Solidity with a fixed supply of 1,000,000 tokens. Includes functionality for token transfers, allowances, and approvals.
MyToken Contract

Overview

MyToken is an ERC20-compliant smart contract built with Solidity, offering a simple implementation of a fungible token. This contract allows users to perform standard ERC20 operations like transferring tokens, approving spending, and checking balances.

Features

Token Name: MyToken

Token Symbol: MTK

Decimals: 18

Total Supply: 1,000,000 MTK


All tokens are initially assigned to the contract deployer.

Functions

Public/External Functions:

1. totalSupply:
Returns the total token supply.


2. balanceOf(address account):
Returns the token balance of a given address.


3. transfer(address recipient, uint256 amount):
Transfers tokens from the caller's address to the recipient.


4. allowance(address owner, address spender):
Returns the remaining amount that a spender is allowed to transfer on behalf of the owner.


5. approve(address spender, uint256 amount):
Approves a spender to transfer up to a specified amount of tokens on the caller's behalf.


6. transferFrom(address sender, address recipient, uint256 amount):
Transfers tokens from one address to another, given the caller has sufficient allowance.


## Events:

+ Transfer:
Emitted when tokens are transferred.

+ Approval:
Emitted when a spender is approved for a specified allowance.


## Deployment
+ Clone the repository and navigate to the directory.


+ Deploy the contract on a supported Ethereum network using Remix, Hardhat, or Truffle.


+ Upon deployment, all tokens will be assigned to the deployer's address.



## Interactions

You can interact with the contract using any Ethereum wallet or development tools like Remix or web3.js.

## Example Usage

+ Transfer Tokens:

myToken.transfer(0xRecipientAddress, 100 * 10**18);


+ Approve Spending:

myToken.approve(0xSpenderAddress, 500 * 10**18);


+ Check Balance:

uint256 balance = myToken.balanceOf(0xAccountAddress);



## Requirements

Solidity ^0.8.0

An Ethereum development environment (e.g., Remix, Hardhat, or Truffle)


License

This project is licensed under the MIT License.

