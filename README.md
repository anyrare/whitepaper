# AnyRare Whitepaper (Draft)

Author: [Panasun Sunanta (Bin)](mailto:panasun@i17.co)

Version: 0.1.0

Last update: Dec 8, 2021

## Abstract

## Table of Contents
- [Introduction](#introduction)
- [Stakeholders](#stakeholders)
- [Physical Assets Tokenization](#physical-assets-tokenization)
- [Incentive Benefit](#incentive-benefit)
- [ARA Pricing Formula](#ara-pricing-formula)
- [Collection Pricing Formula](#collection-pricing-formula)
- [Governance Rules](#governance-rules)
- [Funding Management](#funding-management)
- [Project Roadmap](#project-roadmap)
- [Contributors](#contributors)

### Introduction
Rare items are desirable to collect and invest in because they have sentimental value, are unique and in limited supply, are priced according to the collector's satisfaction, and have a low or no correlation to financial assets returns.

However, due to the nature of this asset class, it is only accessible to a select group of collectors.

- They must be audited by a specialist or curator prior to collection.
- Because they require physical asset transfers and a custodian, investment transactions are restricted.
- They are experiencing liquidity issues (Rich Assets, Poor Cash) as a result of their billions of unique sku; the prices of some of these sku are either too low or too high to invest in.

To address this issue, we propose the AnyRare platform, a decentrailzed platform for the tokenization of tangible assets. This design is based on the [Continous Organization](https://github.com/C-ORG/whitepaper) principle and the [Bancor Formula](https://github.com/Permissionless-Software-Foundation/token-liquidity/blob/master/docs/bancor-formulas/bancor-protocol-whitepaper.pdf) in order to incentive a benefit for all stakeholders.
### Stakeholders
- **Asset Founders:** those who own rare assets and send them to an auditor for minting, as well as storing them with a custodian.
- **Auditors / Curators:** a specialist in that asset class is responsible for certifying rare assets and minting them to the blockchain.
- **Custodians:** who is accountable for storing and delivering a physical rare asset upon request from the asset owner or collector.
- **Collectors:** a non-fungible asset owner who can hold an asset, initiate an auction, withdraw a physical asset, or fractionalize an asset through the creation of a collection.
- **Collection Shareholders:** A fractional stakeholders in a collection who may hold fractional shares in order to earn a capital gain or to earn a profit when the collection is sold to a collector.
- **AnyRare Owner:** anyone who has an ARA token is a fractional owner of the AnyRare platform. That can use their ARA to vote on AnyRare proposals and may receive a portion of the revenue generated by the AnyRare platform. Additionally they can utilize ARA as a medium of exchange to purchase fungible and non-fungible assets and to pay fees on the AnyRare platform.
- **Contributors:** everyone involved in the development of the AnyRare platform, such as founders, developers, business partners, advisers, employees, and influencers.

### Physical Assets Tokenization
The following describes the process of converting rare assets to AnyRare tokens.

1. The asset's owner (Asset Founder) initiates the minting process by sending the physical asset to the auditor. Additionally, they can choose a royalty price for subsequent sales.
2. An auditor certifies an asset, generates an audit report, and creates a non-fungible token on the blockchain using a smart contract.
3. The auditor collects minting costs from the asset's founder and transfers the asset to the custodian.
4. The custodian creates and signs the custodian contract in the blockchain's smart contract. The NFT token will be referred to as the smart contract, and those who own it will be referred to as collectors.
5. As a collector, they can hold an NFT token, launch an auction, withdraw a physical asset, or fractionalize an asset by establishing a collection in order to gain liquidity and collect collector fees when someone buys or sells a share.
6. To build a collection, collectors can specify the target price and collateral weight for any NFT assets in their portfolio to be settled in the collection. Then, using the Bancor Formula, a collection will be built to provide automated liquidity. The collector will receive a full portion of the collection.
7. If a purchaser wishes to acquire a section of this collection. The new share will be automatically generated by the smart contract, and the ARA used to purchase it will be locked in the smart contract as collateral. This procedure can be conducted immediately, without waiting for an offer. Please keep in mind that the number of collector shares will remain constant, but the collection's overall share will increase, diluting the collection portion but increasing the share value.
8. To sell a share, you can automate the process and obtain an ARA that secures in the smart contract. The portion of the collection that you sell will be burned, so decreasing the collection's overall share. Additionally, the Bancor Formula was used to govern the pricing of purchases and sales. Please note that if the value of the sale exceeds the ARA collateral reserved, the seller will get no more than the collateral reserved, and the remaining tokens will be burned to lower the collection's total quantity. This technique is intended to reduce the current collection price; if the current collection price is set too high and does not incentivize an investor, the existing shareholder may burn their token to reduce the current collection price.
9. Once an NFT token has been transformed to a collection, the collector is not permitted to withdraw the asset from the custodian. If someone wishes to withdraw an item from collection, they must bid at least the buyout target price set by the fractional shareholder and the auction procedure will begin.
10. Once a bid is placed at or over the buyout price, the auction will remain open for X days. The auction winner will acquire all NFT assets in this collection, and the ARA from the auction and collateral in the collection smart contract will be distributed equally to collection shareholders. Additionally, this collection will be destroyed. If the collection price is too low in comparison to its true value, this method enabled the arbitrageur to purchase the collection in order to unlock an NFT asset and withdraw from the custodian, at which point they can sell the asset in the real world for its true value.

### Incentive Benefit
AnyRare is designed to be a decentralized organization which anyone can contribute their own resources to its growth. Any party that participates in AnyRare should receive a benefit that is both reasonable and motivating. As a result, we've designed this benefit structure to encourage participation from all parties.

1. Asset Founders:
2. Collectors:
3. Collection Shareholders:
4. Investors:
5. Founders:
6. Developers:
7. Influencers:
8. Auditors / Curators:
9. Custodians:
10. Advisors:

### ARA Pricing Formula
The ARA was using a bonding curve formula to determine the price. To begin minting new ARA tokens, the minter must first transfer the collateral token (DAI) to the ARA smart contract. Then, according to the following formula, the new ARA token will be issued in total supply.

`IssuedToken = ContinuousTokenSupply * ((1 + CollateralTokensReceived / CollateralTokenBalance) ^ (CollateralRatio) - 1)`

The minter will be receive

`MinterPurchaseReturn = IssuedToken * (1 - ManagementRatio)`

Additionally, the remainder of the issued tokens will be distributed for management purposes.

`ManagementFund = IssuedToken * ManagementRatio`

To withdraw, the withdrawer must transfer ARA tokens to the smart contract and will receive collateral tokens according to the formula below.

`WithdrawerSaleReturn = CollateralTokenBalance * (1 - (1 - ContinuosTokensReceived / ContinuousTokensSupply) ^ (1 / CollateralRatio))`

Please keep in mind that this formula will dynamically adjust the overall quantity of ARA tokens based on the collateral tokens locked in the smart contract.

### Collection Pricing Formula

### Governance Rules

### Funding Management
The 1-Collateral of ARA were distributed to management wallets for develop Anyrare platform and ecosystem.

### Project Roadmap

### Contributors
- [Panasun Sunanta (Bin)](mailto:panasun@i17.co) (Lead Developer)
- [Guarantee Pra Co., Ltd.](http://g-pra.com) (Amulet Specialist Partner)
