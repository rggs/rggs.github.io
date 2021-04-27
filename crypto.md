---
layout: default
---


# 1. [Asynchronous 1Inch Prices](https://github.com/rggs/crypto/blob/main/async_1inch_prices.py)  
 My goal with this code was to gain experience with web3 and APIs, in particular a DEX api. The script accesses the 1Inch API and checks to see if any arbitrage
 opportunities exist by choosing different protocol paths through 1Inch. Unsurprisingly, no such opportunities exist, at least in the simple search done in the 
 script. Ultimately the goal was achieved because it provided me greater insight into DEX interactions using python.  


# 2. [ABIs & Contract Interactions](https://github.com/rggs/crypto/blob/main/abi_contract_interactions.py)  
 For this project, I wanted to get the Uniswap V2 pair contracts using direct smart contract interaction through etherscan's API. Although not fast, 
 it does provide a lot of valuable insight into how smart contracts work and how to utilize them. The script calls Uniswap's V2 
 factory contract, gets the total number of pairs, and then iterates through them, recording the contract address and the name of the pair. 
 Following the move from Uniswap V1 to V2, this script slowed down significantly. Going forward, it would be helpful to make this asynchronous 
 like the asynchronous price searcher.
 
 
 
 
