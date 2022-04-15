## Prerequisites ##
Metamask extention (https://metamask.io/)
Remix IDE
Infura account (https://infura.io/)
docker installion (https://docs.docker.com/engine/install/)

## Initial Steps ##
Rename the dotenv file to .env.

To substitute your own details, you will need:
 - An infura account
 - A metamask account with some ropsten ether (put your address and private key in the .env file)
 - To have depoyed the oz_erc20.sol folder from remix (put the deployed contract address in the .env file)

## Executing the DeployedContract.sol
 -Create a project on Remix with .sol extention and rename _name and symbol_ for the DeployedContract.sol file.
 -Select 0.8.8 Compiler and select ERC20 folder for contract and compile the file.
 -Go to Deploy & Run Transactions and select Injected Web3 environment for your Metamask account
 -Deploy the transaction

## Executing the distribute.js
 -Run the below commands to install big-number, contract.js, .env, web3, etherium-tx, dotenv on the terminal
 ```$npm install big-number
 ```$npm install contract.js
 ```$npm install .env
 ```$npm install web3
 ```$npm install etherium-tx
 ```$npm install dotenv
 -You can then run the distribute.js on the terminal by using the below command
```$node .\distribute.js

## Executing the Distribution (using docker) ##
From a terminal running in the same folder as the Dockerfile, run

```$docker-compose up```

This will run the distribution using the configuration details in the .env file.