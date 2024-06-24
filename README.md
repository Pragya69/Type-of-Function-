# Type-of-Function-
# CREATE AND MINT TOKEN

For this project, you will write a smart contract to create your own token on a local HardHat network. Once you have your contract, you should be able to use remix to interact with it. From remix, the contract owner should be able to mint tokens to a provided address. Any user should be able to burn and transfer tokens.
## Introduction

Welcome to the Token (MUK) repository! This repository contains the Solidity smart contract code for the MUK token, an ERC-20 compatible token designed for various purposes. MUK tokens can be used for transactions, rewards, and other activities within an ecosystem.

This README file provides an overview of the MUK token contract and includes instructions on how to deploy the contract to the local Hardhat test network using Remix Connect Localhost and how to interact with it using Remix with Hardhat provider.
## Description

The purpose of this project is to enable users to have full control over their own token by creating a customizable ERC20 token contract. Users can set the name, symbol, and total supply of their token during deployment. The contract owner has the ability to mint new tokens and distribute them to specific addresses. Users can transfer their tokens to other addresses, allowing for peer-to-peer transactions. Additionally, users can burn their tokens if they no longer need them, effectively reducing the token supply.

By providing a flexible and customizable token contract, this project empowers individuals, organizations, and developers to create and manage their own tokens on the Ethereum blockchain. This token can be used for various purposes, such as creating a reward system, facilitating in-app transactions, or launching a new cryptocurrency.

The contract owner has special privileges and is the only address allowed to mint new tokens. Other addresses can interact with the contract by transferring tokens and burning their own tokens.

Contract Name: Token

State Variables:

# name: A public string variable representing the name of the token
# symbol: A public string variable representing the symbol of the token ("MUK").

# decimals: A public uint8 variable representing the number of decimal places for token balance representation (18 decimals).

# totalSupply: A public uint256 variable representing the total supply of tokens.

# balances: A private mapping that maps addresses to their corresponding token balances.

# allowances: A private mapping that maps addresses to allowances granted by token holders to spend tokens on their behalf.

# owner: A public address variable representing the owner of the token contract.
## Getting Started

### Installing

To run the contract, follow these steps:

1. Install the project dependencies by running the following command:

   ```
   npm install
   ```
   2. Start a blockchain locally by running the command: 
   ```
   npx hardhat node
   ```
3. Test the contract by running the command: 
   ```
   npx hardhat test
   ```

4. Deploy the UmarContract smart contract by running the deployment script:

   ```
   npx hardhat run scripts/deploy.js --network localhost
   ```

### Executing program

* Go to [remix](remix.ethereum.org) IDE.
* Paste the contract in the IDE.
* Compile the contract.
* Select the `Dev - Hardhat Provider` as the environment in Deploy tab.
* Paste you contract address in remix and click on `At Address`.
* Play with your contract in remix!!
* ## Interacting with the Contract using Remix with Hardhat Provider

After deploying the MUK token contract to the local Hardhat test network, you can interact with the contract using Remix with Hardhat provider. Here are the steps to get started:

1. Open the [Remix](https://remix.ethereum.org/) online IDE in your browser.

2. In the "File Explorer" section, locate the `Token.sol` file and open it.

3. In the "Deployed Contracts" section, click on the contract named `Token`.

4. In the "At Address" input field, enter the contract address obtained during deployment.

5. Click the "At Address" button to load the contract instance.

6. You can now interact with the RUK token contract through the provided functions.

   - Use the `balanceOf` function to check the token balance of a specific address.
   - Use the `transfer` function to send MUK tokens from your address to another address.
   - Use the `mint` function (accessible only to the contract owner) to mint

 new RUK tokens.
   - Use the `burn` function to burn a specific amount of your RUK tokens.

7. Set the required parameters for each function and click the corresponding button to execute the transaction.

8. Confirm the transaction details and sign the transaction in Remix.

9. Wait for the transaction to be confirmed on the local Hardhat network.

10. You can view the transaction status and emitted events in the Remix console.

## Authors

PRAGYA
https://www.linkedin.com/in/pragya-299103231/
21BCS9346@cuchd.in

## License

This code is released under the MIT License. Feel free to use, modify, and distribute it as per the terms of the license.
