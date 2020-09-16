# The AmpleForthGold Project  

Synthetic Gold forged using Ampleforth technology.

## Project Goals
AmpleForthGold is a decentralized elastic supply protocol based on the [*Ampleforth/uFragments*](https://github.com/ampleforth/uFragments) Implementation. It maintains a stable unit price in gold by adjusting supply directly to and from wallet holders. For a complete description of the protocol and the rationale behind the project, you can read [**the Gold Paper**](https://raw.githubusercontent.com/AmpleForthGold/AmpleForthGold/master/TheGoldPaper.pdf).

## Website
The official [**AmpleForthGold**](https://afgold.org/) website can be found [here](https://afgold.org/). 

## Purchase of AmpleForthGold AAU ERC20 tokens
AmpleForthGold AAU ERC20 tokens can be purchased on [Uniswap](https://app.uniswap.org/#/swap?outputCurrency=0x8E54954B3Bbc07DbE3349AEBb6EAFf8D91Db5734). 

## Key Dates
### 2020/08/25 Initial Token sale, initial liquidity available. (complete!)
On the above date, AmpleForthGold tokens will be available for purchase. Initial liquidity will go live on [*UniSwap*](https://app.uniswap.org/#/swap?outputCurrency=0x8E54954B3Bbc07DbE3349AEBb6EAFf8D91Db5734) on 25th August 2020. This will be 10% of the AAU tokens in existence. The tokens will not be rebased initially and will be freely available to all. Read [**the Gold Paper**](https://raw.githubusercontent.com/AmpleForthGold/AmpleForthGold/master/TheGoldPaper.pdf) for details on the distribution of tokens. 

Exact time shall be 12:12am NZST on 25th August 2020.

### Initial rebasement. (complete!)
The initial rebasement has been moved ***forward*** to 2020/09/08. This is a ***brutal*** rebasement that should align the AAU price with that of gold. A countdown to the rebasement event can be found on our [website here](https://www.afgold.org/rebase-log).

### 2020/09/15 The Rebasement begins. (complete!)
Rebasement of the AAU tokens to the price of one ounce of Gold shall begin. This shall affect the quantity of token you hold, but does not affect the percentage of the market cap you hold. See the original [*Ampleforth Whitepaper*](https://www.ampleforth.org/papers/) for details.

### 2020/09/15 User controlled rebase events. (complete!)
Any user can now generate their own rebase events. Details and a big golden button can be found [here](https://www.afgold.org/rebase-generator).

### 2020/10/15 Midas Launches
Most (90%+) AmpleForthGold tokens will (eventually) be distributed to the holders of AmpleForthGold tokens via Midas. Read [**the Gold Paper**](https://raw.githubusercontent.com/AmpleForthGold/AmpleForthGold/master/TheGoldPaper.pdf) for details on Midas and the distribution of tokens.   

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
The (minimilist) price oracle [RebaseDelta.sol](https://github.com/AmpleForthGold/uFragments/blob/master/contracts/RebaseDelta.sol) can be found at location [0x7d45fd7e1d1afd48da7f10093d8d1ee5dea8cf08](https://etherscan.io/address/0x7d45fd7e1d1afd48da7f10093d8d1ee5dea8cf08) on the ethereum blockchain. 
