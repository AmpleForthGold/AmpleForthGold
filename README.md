# The AmpleForthGold Project  

Synthetic Gold forged using Ampleforth technology.

## Project Goals
AmpleForthGold is a decentralized elastic supply protocol based on the [*Ampleforth/uFragments*](https://github.com/ampleforth/uFragments) Implementation. It maintains a stable unit price in gold by adjusting supply directly to and from wallet holders. For a complete description of the protocol and the rationale behind the project, you can read [**the Gold Paper**](https://raw.githubusercontent.com/AmpleForthGold/AmpleForthGold/master/TheGoldPaper.pdf).

## Website
The official [**AmpleForthGold**](https://afgold.org/) website can be found [here](https://afgold.org/). 

## Purchase of AmpleForthGold AAU ERC20 tokens
[**AmpleForthGold**](https://afgold.org/) AAU ERC20 tokens can be purchased on [Uniswap](https://app.uniswap.org/#/swap?outputCurrency=0x8E54954B3Bbc07DbE3349AEBb6EAFf8D91Db5734). 

## Midas (AmpleForthGold Staking)
[**AmpleForthGold**](https://afgold.org/) AAU can be staked on [**Midas**](https://www.afgold.org/staking).

## Project milstones
Project milestones are maintained on our primary website: [**AmpleForthGold**](https://www.afgold.org/roadmap).

## ERC20 Rebasing Contract
This repository is a collection of smart contracts that implement the AmpleForthGold protocol on the Ethereum blockchain.
### Mainnet (Ethereum Blockchain)
#### ERC20 Token Location ([UFragments.sol](https://github.com/AmpleForthGold/uFragments/blob/master/contracts/UFragments.sol))
> (contract proxy interface) [0x8E54954B3Bbc07DbE3349AEBb6EAFf8D91Db5734](https://etherscan.io/address/0x8E54954B3Bbc07DbE3349AEBb6EAFf8D91Db5734)<br>
> (contract implementation) [0x64cb197240876c32e68d2d17b405b7bf92ed523f](https://etherscan.io/address/0x64cb197240876c32e68d2d17b405b7bf92ed523f)

## Token Holders
|Holder|Quantity|Address|
|:---|:---|:---|
|Midas Locked Pool| >=90% of AAU| [0xaea0a086ce5584cdffce2930497b38c937cbb24e](https://etherscan.io/token/0x8E54954B3Bbc07DbE3349AEBb6EAFf8D91Db5734?a=0xaea0a086ce5584cdffce2930497b38c937cbb24e)|
|Uniswap Liquidity Pool | >=10% of AAU| [	0x173015cf1260f1fa024bde2e08845aed61c99e3b](https://etherscan.io/token/0x8E54954B3Bbc07DbE3349AEBb6EAFf8D91Db5734?a=0x173015cf1260f1fa024bde2e08845aed61c99e3b)|

### Uniswap/Unicrypt locked liquidity
Liquidity was provided to uniswap on 2020/08/25 by the founding members of AmpleForthGold. That Uniswap liquidity has been locked on [Unicrypt](https://unicrypt.network/uniswap-browser/pair/0x2d0C51C1282c31d71F035E15770f3214e20F6150). The release dates are staggered over a period of 5 months. The release dates are an estimate based on calculations and as per the details outlined in [**the Gold Paper**](https://raw.githubusercontent.com/AmpleForthGold/AmpleForthGold/master/TheGoldPaper.pdf).

## Rebase Design Information
The Primary Rebase contract is called [Orchestrator.sol](https://github.com/AmpleForthGold/uFragments/blob/master/contracts/Orchestrator.sol). It can be found on the ethereum blockchain at address [0xa3484d111abb94c21638c526d97db9cd9e5a0b2a](https://etherscan.io/address/0xa3484d111abb94c21638c526d97db9cd9e5a0b2a). Further details can be found in the [rebase design notes](https://raw.githubusercontent.com/AmpleForthGold/AmpleForthGold/master/ReBasePaper.pdf). 

## Price oracle
The (minimalist) price oracle [RebaseDelta.sol](https://github.com/AmpleForthGold/uFragments/blob/master/contracts/RebaseDelta.sol) can be found at location [0x7d45fd7e1d1afd48da7f10093d8d1ee5dea8cf08](https://etherscan.io/address/0x7d45fd7e1d1afd48da7f10093d8d1ee5dea8cf08) on the ethereum blockchain. 

## MIDAS
### Midas Distributor
The Midas distributor contract can be found at [0xaea0a086ce5584cdffce2930497b38c937cbb24e](https://etherscan.io/address/0xaea0a086ce5584cdffce2930497b38c937cbb24e). The Midas distributor shall hold the locked pool of AAU tokens to be distributed via Midas Staking Agents. 

### Midas Agents
1. The Midas Agent for AAU (AAU) is located at [0x184B9614C46db115815fac4707B36347B98acfb3](https://etherscan.io/address/0x184B9614C46db115815fac4707B36347B98acfb3)
2. The Midas Agent for AAU-ETH-v2 is located at [0x02Fc1453473a1FcCc2ac2D5f50aE5a933AFEc26e](https://etherscan.io/address/0x02Fc1453473a1FcCc2ac2D5f50aE5a933AFEc26e)
2. The Midas Agent for AAU-PAXG-v2 is located at [0xBEf9348fEE6827D89f4a9767c64b3944D077fd20](https://etherscan.io/address/0xBEf9348fEE6827D89f4a9767c64b3944D077fd20)
2. The Midas Agent for AAU-PMGT-v2 is located at [0x9931A24985A1C553D3D24368C19a4a46a8B174Db](https://etherscan.io/address/0x9931A24985A1C553D3D24368C19a4a46a8B174Db)
2. The Midas Agent for AAU-AMPL-v2 is located at [0xAa17eA7765c6056f2009888F3e77294885c1fA82](https://etherscan.io/address/0xAa17eA7765c6056f2009888F3e77294885c1fA82)

The AAU Agent shall go live at 8pm Tuesdays 6th October 2020 GMT. Other agents will follow progressivly. 

## Liquidity Pools
AAU has several UniSwap-V2 pools that can be used to buy/sell AAU.
|Pair|Description|Address|
|:---|:---|:---|
|AAU-ETH-v2| Ethereum exchange|[0x2d0c51c1282c31d71f035e15770f3214e20f6150](https://etherscan.io/address/0x2d0c51c1282c31d71f035e15770f3214e20f6150)|
|AAU-PMGT-v2| Perth Mint Gold Token Exchange| [0x15f7b9a0c5fe2f33d3dbdf1bcdb1f6dc7bed10b1](https://etherscan.io/address/0x15f7b9a0c5fe2f33d3dbdf1bcdb1f6dc7bed10b1)|
|AAU-AMPL-v2| Ampleforth Exchange|[0xcdc3d2c8c79091b9b63a70a98716e3b40d1299d4](https://etherscan.io/address/0xcdc3d2c8c79091b9b63a70a98716e3b40d1299d4)|
|PAXG-AAU-v2| PAX Gold Exchange |[0x225c01e8c5310714bcb8e8cef68d5814348efdeb](https://etherscan.io/address/0x225c01e8c5310714bcb8e8cef68d5814348efdeb)|
