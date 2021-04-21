# Hardhat Fork for Testing Chess Pieces

## Installing
1. Download this repo: `git clone https://github.com/coin-artist-project/chess-hardhat-fork`
1. Enter the directory: `cd ./chess-hardhat-fork`
1. Install the dependencies: `npm install`

## Set the config
1. Copy `.env.SAMPLE` into `.env` and add your Alchemy API key (can get a free one at alchemyapi.io)
1. Open `scripts/send-chess-pieces.js` and update the variable `SEND_TO_DEST_ADDRESS` to point to your Metamask address

## Running 

1. Open a second terminal window
1. In the first terminal window, start up a local Ethereum fork of mainnet: `npm run fork`
1. In the second window, transfer chess pieces to you (fork must be running, takes around 5-10 seconds to finish): `npm run sendBatchItems`

## Using in Metamask

1. Add the hardhat local configuration to your Networks in Metamask
1. Configuration:
	- Network Name: `Hardhat Local`
	- RPC URL: `http://127.0.0.1:8545`
	- Chain ID: `31337`
	- Currency Symbol: `ETH`

![Metamask instructions image](hardhat-local-metamask.png?raw=true)
