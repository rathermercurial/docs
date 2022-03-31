---
description: >-
  Summary of Aave Improvement Proposal: "Add alUSD as a Borrowable Asset on Aave
  V2" for RabbitHole Metagovernance Pod.
---

# Aave - alUSD Listing Supplemental

This document was created to serve as a supplemental content related to [Aave proposal: Add alUSD as a Borrowable Asset on Aave](https://snapshot.org/#/aave.eth/proposal/0x825785609d88dda63b41255aa0137ead680f02eb4f7387219b0969a1102b0746), submitted 2/16/21 to Aave Governance via Snapshot.org. Written for the Rabbithole Metagovernance Pod by [rathermercurial.eth](https://rathermercurial.eth.xyz) on 1/17/22.

### Proposal Summary

The Alchemix Finance Core Team has proposed the addition of alUSD ("Alchemic USD") as a _borrowable asset_ in the Aave v2 protocol. Their goal in doing so is to better establish alUSD as a reliable, resilient and highly liquid stablecoin throughout the DeFi ecosystem. Alchemix has also expressed interest in incorporating Aave liquidity markets into its yield-earning strategy, potentially bringing deep, reliable alUSD liquidity to Aave and new revenues to both protocols. This proposal does _not_ allow for alUSD to be used as collateral on Aave.

> The purpose of this AIP is to list alUSD as a borrowable asset on Aave. alUSD has established itself as one of the leading new stablecoins in terms of stability and liquidity, and listing on Aave will provide users with a proven stablecoin to borrow. Alchemix has 376m TVL in the form of yvDAI and DAI backing alUSD, with a liquid supply of 239m alUSD. alUSD has one of the deepest Curve pools, with \~450m in liquidity. In addition to the Curve pool, alUSD has additional liquidity on Sushiswap, Saddle, and mStable. According to Parsec Finance’s StableRank, alUSD is routinely among the top stablecoins in terms of price stability and liquidity within 1% slippage. Having been on the market for over 6 months while maintaining the peg through turbulent market conditions, alUSD has built the reputation required to be an asset listed on AAVE. --[_Alchemix Core Team_](https://snapshot.org/#/aave.eth/proposal/0x825785609d88dda63b41255aa0137ead680f02eb4f7387219b0969a1102b0746)

Alchemix believes alUSD to be a desirable asset to borrow due not only to its noteworthy performance as a debt-collateralized stablecoin (similar to DAI), but also due to their generous farming incentives, arbitrage opportunities and utility within supported protocols such as Alchemix, Premia and more. Aave users will gain access to a variety of risk-averse strategies to maximize their yield and manage debt positions across both platforms.

#### Risks and Security Considerations

This proposal would introduce new protocol risk to Aave v2 from the Alchemix, alUSD and Yearn Vault contracts. This type of risk is common to all new assets, and is minimized by restricting users from borrowing against their alUSD deposits. There is no mention of allowing alUSD to be used as collateral in the future.

At this time, the value of alUSD is fully backed by, and pegged to, the Dai stablecoin. Aave has already assigned Dai an overall rating of "B+" in their own internal risk analysis. Alchemix will be adding USDC and USDT (rated "A-" and "B+", respectively) strategies at a later date, at a robust minimum collateralization rate of \~157%.

The Alchemix admin multisig should also be considered a risk factor, as it can be used to mint alUSD, grant minting permission to other contracts, and update contract parameters such as the debt cap, collateralization ratio and fee percentage. Each member of the Alchemix core team also has the ability to pause the main alchemist.sol contract in the case of an emergency.

#### Implementation

If this vote passes, the Alchemix team will make a pull request to the Aave Github Repository, containing the payloads necessary to add alUSD to the assets list. Alchemix will also furnish Chainlink price oracles which are already widely used for alUSD by protocols such as Curve, Sushi and mStable. This is noteworthy, as many other recent asset listing proposals have lacked a similar degree of planning, effort and investment in the Aave ecosystem.

***

**Specifications**

Borrowing Enabled ✅

Reserve Factor: 20%

Liquidation Bonus: 0%

Liquidation Threshold: 0%

Base LTV as Collateral: 0%

_Cannot Be Used as Collateral ❌_

***

**Aave Governance RFC & Proposal 👇**

Active Snapshot.org Proposal: https://snapshot.org/#/aave.eth/proposal/0x825785609d88dda63b41255aa0137ead680f02eb4f7387219b0969a1102b0746

Aave Governance Discussion: https://governance.aave.com/t/arc-add-alusd-as-borrowable-to-aave-v2/7191

***

### About Alchemix and alUSD

Alchemix Finance is a Future Yield Tokenization (commonly known as "Self-Repaying Loan") protocol built on the Ethereum blockchain which issues over-collateralized loans in the form of 1:1 pegged synthetic assets (alUSD & alETH). Users can deposit Dai or Ether (with more assets coming soon) to obtain a loan which repays itself over time, without the need for compounding or position management, nor risk the risk of accidental liquidation.

> Alchemix is an evolution of the tried and true CDP model trailblazed by MakerDAO. Alchemix is, at its core, an overcollateralized stablecoin, much like DAI and other similar tokens. It has some key differences however.
>
> Alchemix only mints like-kind or “mirror” al-Assets. For example, alUSD is only mintable by DAI (and later USDT and USDC), and alETH is only mintable by ETH (and later other ETH derivatives). Deposited collateral is then deployed to yearn, of which the earned yield doubly repays users’ debt and backs the dollar peg in the Transmuter module. In addition, there is no interest paid in the borrowing of al-Assets. Due to this structure, Alchemix does not have liquidations in its system. This allows people to maximum borrow without fear of shifting market conditions - taking an essentially risk free negative interest alUSD loan with their DAI. In effect, the system acts as a way to get an advance on your yield for your stablecoin deposits.
>
> \--[_Alchemix Core Team_](https://snapshot.org/#/aave.eth/proposal/0x825785609d88dda63b41255aa0137ead680f02eb4f7387219b0969a1102b0746)

Alchemix is currently one of the largest liquidity providers on Yearn Finance, and their governance token, $ALCX, is widely listed on exchanges such as Coinbase, Binance and FTX, with a market cap of \~$170M. A significant portion of its DeFi liquidity is protocol-owned thanks to their early partnership with Olympus Pro.

#### How alUSD Works:

Alchemix maintains the alUSD peg via several methods including conservative, DAO-governed debt caps, a _50%_ LTV (Loan-to-Value) ratio, Governance incentives for alUSD liquidity providers, and a variety of tools for users to manage their positions and profitably arbitrage the alUSD / Dai exchange rate. This strategy has proven incredibly robust, resulting in outstanding stability during all market conditions (sometimes outperforming even legacy fiat-collateralized stablecoins during times of peak volatility).

In order to provide adequate interest rates and to ensure stability of the alUSD peg, loans on Alchemix are always over-collateralized by 100%. Borrowers may choose to repay their loan with Dai or alUSD, or they can simply collect interest in the form of repaid debt minted by the protocol directly to the borrower's CDP. alUSD obtained as repaid debt is _not_ over-collateralized, thus providing an incentive for borrowers to hold their debt positions (rather than paying loans off quickly, as one might pay a tradfi loan). This ultra-low LTV ratio is key to alUSD's performance:

> alUSD minted from a new loan has a collateralization ratio of 200%, while alUSD minted from repaid debt has a collateralization ratio of 100%. The total global collateralization ratio for alUSD is 157%. The supply can expand in two ways – an expansion in the debt ceiling followed by users taking new loans, or debt repayments with DAI, which decrement the global debt while not destroying alUSD. This is how we have a supply of \~239m with a current debt cap of 150m. alUSD can be burned by staking it in the transmuter, where it is converted 1:1 to DAI over time.. --[_Alchemix Core Team_](https://snapshot.org/#/aave.eth/proposal/0x825785609d88dda63b41255aa0137ead680f02eb4f7387219b0969a1102b0746)

Alchemix currently achieves its base yield by depositing collaterals into Yearn v2 Vaults, and as mentioned in this proposal, are exploring other sources of revenue including deposits to the proposed Aave v2 alUSD market. Such a synergy between Aave and Alchemix would likely create a net-positive impact for both protocols in terms of overall utility, revenue and TVL across the board.

### Important Links:

_Alchemix Finance Official Website:_ https://alchemix.fi/

Alchemix Whitepaper: https://alchemix.fi/c76d1d663f6c8247b86a8fca83d5bd1b.pdf

Alchemix Docs: https://alchemix-finance.gitbook.io/alchemix-finance/

Alchemix Github: https://github.com/alchemix-finance

Protocol Audit by Certik: https://alchemix.fi/a208baf6ca7e0d6b0116461f05e27cd9.pdf

$alUSD Token Contract on Etherscan: https://etherscan.io/token/0xbc6da0fe9ad5f3b0d58160288917aa56653660e9

$alUSD Asset Details on CoinGecko: https://www.coingecko.com/en/coins/alchemix-usd
