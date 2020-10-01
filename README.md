# The AmpleForthGold Project  

Synthetic Gold forged using Ampleforth technology.

## Project Goals
AmpleForthGold is a decentralized elastic supply protocol based on the [*Ampleforth/uFragments*](https://github.com/ampleforth/uFragments) Implementation. It maintains a stable unit price in gold by adjusting supply directly to and from wallet holders. For a complete description of the protocol and the rationale behind the project, you can read [**the Gold Paper**](https://raw.githubusercontent.com/AmpleForthGold/AmpleForthGold/master/TheGoldPaper.pdf).

## Website
The official [**AmpleForthGold**](https://afgold.org/) website can be found [here](https://afgold.org/). 

## Purchase of AmpleForthGold AAU ERC20 tokens
AmpleForthGold AAU ERC20 tokens can be purchased on [Uniswap](https://app.uniswap.org/#/swap?outputCurrency=0x8E54954B3Bbc07DbE3349AEBb6EAFf8D91Db5734). 

## Project milstones
Project milestones are maintained on our primary website: [**AmpleForthGold**](https://www.afgold.org/roadmap).

## ERC20 Rebaseing Contract
This repository is a collection of smart contracts that implement the AmpleForthGold protocol on the Ethereum blockchain.
### Mainnet (Ethereum Blockchain)
#### ERC20 Token Location ([UFragments.sol](https://github.com/AmpleForthGold/uFragments/blob/master/contracts/UFragments.sol))
> (contract proxy interface) [0x8E54954B3Bbc07DbE3349AEBb6EAFf8D91Db5734](https://etherscan.io/address/0x8E54954B3Bbc07DbE3349AEBb6EAFf8D91Db5734)<br>
> (contract implementation) [0x64cb197240876c32e68d2d17b405b7bf92ed523f](https://etherscan.io/address/0x64cb197240876c32e68d2d17b405b7bf92ed523f)

## Token Holders
|Holder|Quantity|Address|
|:---|:---|:---|
|Founders (Midas)|45000000| [	0x0f9dd348cdbde17f27f63d4a985f70c2e2beedd5](https://etherscan.io/token/0x8E54954B3Bbc07DbE3349AEBb6EAFf8D91Db5734?a=0x0f9dd348cdbde17f27f63d4a985f70c2e2beedd5)|
|Founders (Uniswap Liquidity) |5000000| [	0x173015cf1260f1fa024bde2e08845aed61c99e3b](https://etherscan.io/token/0x8E54954B3Bbc07DbE3349AEBb6EAFf8D91Db5734?a=0x173015cf1260f1fa024bde2e08845aed61c99e3b)|

### Uniswap/Unicrypt locked liquidity
Liquidity was provided to uniswap on 2020/08/25 by the founding members of AmpleForthGold. That Uniswap liquidity has been locked on [Unicrypt](https://unicrypt.network/uniswap-browser/pair/0x2d0C51C1282c31d71F035E15770f3214e20F6150). The release dates are staggered over a period of 5 months. The release dates are an estimate based on calculations and as per the details outlined in [**the Gold Paper**](https://raw.githubusercontent.com/AmpleForthGold/AmpleForthGold/master/TheGoldPaper.pdf).

### Midas AAU Tokens locked 
100% of the Midas AAU tokens (45000000) were locked using contract [0x34628b19f2267f31e4aCEe652A234216903e2385](https://etherscan.io/address/0x34628b19f2267f31e4acee652a234216903e2385#code). They have been locked until 22nd of September 2020.

## Rebase Design Information
The Primary Rebase contract is called [Orchestrator.sol](https://github.com/AmpleForthGold/uFragments/blob/master/contracts/Orchestrator.sol). It can be found on the ethereum blockchain at address [0xac5f9327a89523c09cf38be79f65f3220511e8b9](https://etherscan.io/address/0xac5f9327a89523c09cf38be79f65f3220511e8b9). Further details can be found in the [rebase design notes](https://raw.githubusercontent.com/AmpleForthGold/AmpleForthGold/master/ReBasePaper.pdf). 

## Price oracle
The (minimalist) price oracle [RebaseDelta.sol](https://github.com/AmpleForthGold/uFragments/blob/master/contracts/RebaseDelta.sol) can be found at location [0x7d45fd7e1d1afd48da7f10093d8d1ee5dea8cf08](https://etherscan.io/address/0x7d45fd7e1d1afd48da7f10093d8d1ee5dea8cf08) on the ethereum blockchain. 

## uFragments (ERC20) proxy burning
Ampleforth recently decided to deploy a new contract because of the recent KuCoin Hack. The new contract blocked certain addresses associated with the KuCoin hack. The AmpleForthGold team are opposed to that sort of behaviour as it allows for governments and/or powerful entities to interfere with the supply of an ERC20 token. It also allows for an unlimited rug-pull at any time. With this sort of proxy, it does not matter if you hold your private keys, because the contract owners can take your coins whenever they feel like it. 

The AmpleForthGold implementation uses the same openzeppelin proxy as the original Ampleforth project. Thus, as it currently stands, the AmpleForthGold Project could (at any time) deploy a new ECR20 contract that changes pretty much any aspect of the AAU token. That was fine when we were still in a development phase, but we believe that the ERC20 code for AmpleForthGold is now solid enough to allow us to 'burn the ownership keys' for the openzepplin proxy. 

The AmpleForthGold team will burn the uFragments proxy keys in the next few weeks once we have done a proper internal audit of the codebase. This should happen before the end of October 2020. Once this is done then your tokens are your tokens - we will not be able to help you if you lose your keys or send your tokens to the wrong address. 

## MIDAS
### Midas Distributor
The Midas distributor contract can be found at [0xaea0a086ce5584cdffce2930497b38c937cbb24e](https://etherscan.io/address/0xaea0a086ce5584cdffce2930497b38c937cbb24e). The Midas distributor shall hold the locked pool of AAU tokens to be distributed via Midas Staking Agents. 

### Midas Agents
1. The Midas Agent for AAU (AAU) is located at [0x184B9614C46db115815fac4707B36347B98acfb3](https://etherscan.io/address/0x184B9614C46db115815fac4707B36347B98acfb3)
2. The Midas Agent for AAU-ETH-v2 is located at [0x02Fc1453473a1FcCc2ac2D5f50aE5a933AFEc26e](https://etherscan.io/address/0x02Fc1453473a1FcCc2ac2D5f50aE5a933AFEc26e)
2. The Midas Agent for AAU-PAXG-v2 is TBD.
2. The Midas Agent for AAU-PMGT-v2 is TBD.
2. The Midas Agent for AAU-AMPL-v2 is TBD.

All Midas Agents are currently locked and cannot be used. They will be unlocked once final verification has occurred, and a formal announcement made. 

