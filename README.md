# How to deploy a contract in XDC Network (Apothem / Mainnet)
## Powered by Plugin(A decentralized Oracle)

This guide will give you a clear direction on how to deploy your smart contract in Mainnet / Apothem

if any queries / comments, feel free to raise an issue.

## pre-requisites
- nvm version 0.37.2
- npm version 7.24.0
- node version 16.10.0
- do seup XDCPay Chrome Extension in your chrome 
- setup Hardhat (https://www.npmjs.com/package/hardhat)

## How it works?
- Copy down your contract in contract folder
- Update deplooyment script under scripts/ folder to refer your contract name
- Pass necessary constructor parameter if any
- If you have more than one contract to deploy, then refer those accordingly
- Pass your PRIVATE_KEY in .env to deploy your contract against specific network ( Apothem or Mainnet)

## .env should have following parameters
- PRIVATE_KEY(of your account) to migrate the contract

## How to RUn
- do git clone & npm install or yarn

``` 
 npm install  or yarn
```
## How to deploy sample contract
```
yarn deploy --network apothem  

or 

yarn deploy --network mainnet
```
this will deploy the contract in apothem network and contract address will be stored in output.json