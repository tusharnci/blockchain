
# Blockchain Concept 

In this project we are going to deploy a ERC20 Token on the Ropsten Network and using Node js we are going to distribute it to 10 other metamask accounts.

To get started with the project we first need to create 11 metamask accounts i.e. 1 will be your main account and other 10 will be your distribution accounts.


## Deployment
Pre-requisites:

First we install node.js and vs code for the Deployment. 

Then we check the node version in Visual Studio Code Editor



## Installation

Version Check

```bash
  node --version
```
Once the node modules are created we need to deploy the smartcontract usig remix ethereum editor.

Copy the deploymentcontract.sol code to remix IDE and edit the token name as per your need.

After editing the token, its time to deploy the contract.

Click on the solidity compiler and select 0.8.0 and click on compile.

After that click on the Deploy & run transactions button and select Injected Web3 as the environment.

Your metamask account will open on the right and will ask for authentication.

Select the custom token contract and click on deploy, metamask will open and will ask to confirm the transaction.

## Roadmap

Once your transaction is complete you will open the contract on etherscan and copy the contract address to import the tokens.

Once you import the custom tokens into your account come back to the VS code terminal

```bash
  npm i fs big-number dotenv web3 ethereumjs-tx
```

Now you have to setup env file in which your Infura project id,contract address, owner address, private key has to be pasted.

Now Run

```bash
  node distribute.js
```

Once the code is executed 5% of the tokens from total tokens will be distributed to 10 different metamask accounts.


