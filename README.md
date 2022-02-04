# Joint Savings Account Smart Contract

This repo demonstrates a basic example of enabling functionality for a joint savings account on the Ethereum blockchain through a smart contract.  For demo purposes the smart contract can accept two joint ownership payable addresses that can be withdrawn to  using a method that both validates ownership and contract balance.  Contract balances are set through both a payable deposit method and an external payable fallthrough function.

## Technologies

The application uses the following technologies:

- [Solidity v. 0.5.0](https://docs.soliditylang.org/en/v0.5.0/)
- [Remix IDE](https://remix.ethereum.org/)

## Installation Guide for Demo

### Remix IDE

These instructions assume prior experience with Remix:

- Navigate to [Remix](https://remix.ethereum.org/)
- Load **JointSavings.sol** into the Workspace
- Compile
- Deploy to a JavaScript VM

## Overview

### Objective

The objective of this tool is to demo how a smart contract can govern the rules around a joint savings account.

### Deployment

![Screenshot of deploy](images/001_deploy.png)

### Deposits

Deposits to the contract used the Deposit method.

- Initial deposit of 1 ETH as Wei (1_000_000_000_000_000_000):

![Screenshot of deposit of 1 ETH](images/002_deposit_1eth_as_wei.png)

- Additional deposit of 10 ETH as wei (10_000_000_000_000_000_000)

![Screenshot of deposit of 10 additional ETH](images/003_deposit_10eth_as_wei.png)

- Last deposit of 5 ETH

![Screenshot of deposit of 5 additional ETH](images/004_deposit_5eth_as_eth.png)

### Configuring Accounts

The joint owner addresses were configuring using the setAccounts method:

![Screenshot of ownership accounts](images/005_setAccounts.png)

### Withdrawals

- Transferring 5 ETH to Account 1

![Screenshot of transferring 5 ETH to Account 1](images/006_transfer_5eth_to_accountOne.png)

- Transferring 10 ETH to Account 2

![Screenshot of transferring 10 ETH to Account 2](images/007_transfer_10eth_to_accountTwo.png)

- Insufficient funds example

![Screenshot of insufficient funds](images/008_insufficient_funds.png)

- Unauthorized example

![Screenshot of insufficient funds](images/009_unauthorized_user.png)

## Contributors

- Jacob Rougeau

## License

MIT
