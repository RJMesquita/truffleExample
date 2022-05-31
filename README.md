# Truffle Simple Storage Example
## This is a beginner guide for Truffle based on the video of EatTheBlocks with some personal notes. 

## Truffle Tutorial for Beginners | Compile, Test & Deploy Smart contracts to any EVM Blockchain
https://www.youtube.com/watch?v=62f757RVEvU

## Syntax: 
* **truffle init** - start a new project with truffle;
  * This project will have 3 folders and a file: 
    * **contracts:** were the smart contracts are developed; 
    * **migrations:** file that will migrate the smart contract into the blockchain; 
    * **test:** were you can develop the tests for your smart contract before its deployed;
    * **truffle-config.js:** configuration file for all the project (networks, mocha and compilers).
* **truffle compile** - compile your smart contracts;
  * **Note:** it is necessary to manually  configure the compiler in the truffle-config.js; 
* **truffle test** - deploy your tests for the smart contracts in the .js file;
* **truffle develop** - An interactive console that also spawns a development blockchain;
* **migrate --reset** - migrates your smart contract with ganache;
* **truffle migrate** - migrates your smart contract into the blockchain; 
* **truffle migrate --network kovan** - migrates the smart contract into the kovan network; 
* **truffle console** -  A basic interactive console connecting to any Ethereum client;
* **truffle console --network  kovan** - connecting to the kovan network;
  * **Note:** for both console and migrate it is necessary to configure the privateKey and the network in the truffle-config.js; 

## Execute commands: 
* storage = await SimpleStorage.deployed()
* storage.address - contract address 
* await storage.updateData(29)
*  data = await storage.readData()
* data.toString()
