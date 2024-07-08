# Ethernaut Solution

This project aims to record solutions for challenges on [ethernaut](https://ethernaut.openzeppelin.com/). \
On ethernaut, it is available to solve some levels only using browser setups, but often needs tools outside browser, such as truffle or remix. \
So I thought reproducable, sharable, recordable project would help some people on new to ethernaut.

## requirement
Only thing you need is truffle!
```bash
bash> sudo npm install truffle -g
```

## project structure

project is created by using `web3.js` + `truffle`.

- contracts: solidity smartcontracts will be placed.
- scripts: helper scripts will be placed.
- scripts\/<level-title\>: solution of level.

## environment
You have to create .env first, just copy .env.example!
``` bash
bash> cp .env.example .env
```
Fill variables!
```bash
PRIVATE=blah-blah
WSRPC=wss://polygon-mumbai-bor.publicnode.com
```

## Run
Check commands using --help option
```bash
# run command
npm run start -- --help
# deploy
npm run start -- deploy CoinFlip
# deploy with arguments
npm run start -- deploy CoinFlipHack --args 0x6993Db3723F321003f8a047DB7E49fAcd0ce6390
# execute script
npm run start -- execute CoinFlip --args 0x6993Db3723F321003f8a047DB7E49fAcd0ce6390
```