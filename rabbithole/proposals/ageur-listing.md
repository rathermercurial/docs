---
description: >-
  Summary of Aave Improvement Proposal: "Add agEUR on Aave V3 on Polygon" for
  RabbitHole Metagovernance Pod.
---

# Aave - agEUR Listing Supplemental

This document was created to serve as a supplemental content related to [Aave proposal: Add agEUR on Aave V3 on Polygon (snapshot.org)](https://snapshot.org/#/aave.eth/proposal/0xcb0f6e30a4fdab381962184bd37223a933f120d8158a9f929efd1dc96b3fa392), submitted 2/20/21 to Aave Governance via Snapshot.org. Written for the Rabbithole Metagovernance Pod by [rathermercurial.eth](https://rathermercurial.eth.xyz) on 2/21/22.

Nothing about this document should be considered an endorsement or recommendation of any protocol, asset, etc. This information is only here to assist you in Doing Your Own Research. Please vote responsibly. 🤘

## AIP: Add agEUR on Aave V3 on Polygon

### Proposal Summary

The Angle Protocol Core Team has proposed the listing of their Euro-pegged stablecoin, $agEUR (or "Angle Euro"), on Aave v3 pending its release on Polygon network. According to their proposal, their goal is to provide yield-earning opportunities to $agEUR holders, and access to Euro-denominated leverage for crypto assets (ETH, wBTC, etc.) to Aave users.

> As for the overall benefit of agEUR for the Aave community, many agEUR holders are looking for a reliable place to deposit their stablecoins and get a simple yield on this. Aave would provide this use case. More generally, many DeFi farmers are coming from Europe and want to get a yield on their home currency without being exposed to a USD/EUR change risk. Listing agEUR on Aave would open the gates for many institutional players coming to get yield on their €.

**Proposed By:** [Angle Core Team](https://www.angle.money)\
**Start Date:** 2/20/22 | **End Date:** 2/23/22\
**Forum Discussion: (RFC)**: [https://governance.aave.com/t/listing-proposal-add-ageur-on-aave-v3-on-polygon/7325](https://governance.aave.com/t/listing-proposal-add-ageur-on-aave-v3-on-polygon/7325)\
**Snapshot.Org Vote (AIP):** [https://snapshot.org/#/aave.eth/proposal/0xcb0f6e30a4fdab381962184bd37223a933f120d8158a9f929efd1dc96b3fa392](https://snapshot.org/#/aave.eth/proposal/0xcb0f6e30a4fdab381962184bd37223a933f120d8158a9f929efd1dc96b3fa392)

#### Risks and Security Considerations

$agEUR is overcollateralized and backed by a pool of USDC, Dai, FEI and Frax, which are listed on Aave with risk analysis scores of from C- to A-. There is no relevant risk analysis available for comparison on Aave since agEUR is a novel stablecoin model and is Euro-denominated. [Crypto Risk Assessments](https://cryptorisks.substack.com/p/ageur-angle-protocol) has published an extensive risk analysis related to Curve, in which they recommended that agEUR should receive a gauge.

AgEUR is governed by a DAO of $veANGLE holders, whose votes are implemented using a 4/6 multisig owned by 3 Angle core team members and 3 community members. This multisig _cannot_ be used to min agEUR, but can be used to upgrade the agEUR minting contract. [3 security audits](https://docs.angle.money/resources/audits) have been performed by Chainsecurity and Sigma Prime.

#### Implementation

There is no proposed plan for the implementation of agEUR if this proposal passes (presumably due to the fact that Aave v3 is not yet implemented). The proposal makes no mention of a timeline, or how the proposed changes will be implemented.

There is no Chainlink oracle for agEUR, though the Angle team claims they have met all security compliance requirements and that: "If this Snapshot vote is positive, then the Chainlink team could setup this oracle pretty rapidly".

#### **Proposed Parameters:**

Angle has proposed three parameter models for the agEUR market on Polygon: Isolation Mode, v3 Efficiency Mode Stablecoins and a hypothetical "v3 Efficiency Mode EUR Stablecoins", each with varying parameters. There is no mention as to how the final parameters will be determined (i.e. by snapshot vote or otherwise).

* _Borrowing Enabled ✅_
* Reserve Factor: 10-20%
* Base LTV as Collateral: 80-97%
* Liquidation Threshold: 80-98%
* No Specified Liquidation Bonus
* _Can Be Used as Collateral ✅_

### About Angle Protocol & agEUR

Deployed in November of 2021, agEUR is a novel derivatives exchange and stablecoin protocol which provides alternative forms of stable assets which are overcollateralized and can be minted in a capital-efficient manner.

Angle offers native, leveraged perpetual contracts and a variety of $USD / $EUR arbitrage opportunities to incentivize hedging agents and liquidity providers to maintain the agEUR peg. In short, Angle protocol provides stablecoin seekers, arbitrageurs and yield farmers a platform where they work _together_ to create sustainable, accessible alternatives to typical USD-denominated stables.

> Angle Protocol is a decentralized stablecoin protocol designed to be both over-collateralized and capital-efficient.\
> The protocol has started by launching agEUR, a Euro stablecoin in November.... agEUR can at the moment only be issued on Ethereum mainnet, but it can be bridged on many different chains, like on Polygon... Fantom, Harmony, BSC, Avalanche, Solana, NEAR, Aurora and Fuse.\
> \
> \--[Angle Core Team](https://snapshot.org/#/aave.eth/proposal/0xcb0f6e30a4fdab381962184bd37223a933f120d8158a9f929efd1dc96b3fa392)

agEUR has shown relatively strong performance and stability relative to other Euro-denominated stables, which sometimes struggle to maintain adequate liquidity and stability due to slower adoption, lack of regulatory clarity and other reasons. agEUR has reached a market cap of over $128M in just four months, but only $8M has been bridged to Polygon. The Angle Protocol currently has a TVL $227M and an overall collateral ratio of \~155%.

#### Important Links:

* [Angle Protocol Official Website](https://www.angle.money)
* [Angle Whitepaper](https://docs.angle.money/whitepaper)
* [Angle Docs](https://docs.angle.money)
* [Angle Protocol Github](https://github.com/AngleProtocol)
* [Angle Protocol Audits](https://chainsecurity.com/security-audit/angle-protocol/)
* [Dune Analytics Dashboard](https://analytics.angle.money/#/home)
* [$agEUR Token Contract on Etherscan](https://etherscan.io/address/0x1a7e4e63778b4f12a199c062f3efdd288afcbce8)
* [$agEUR Asset Details on CoinGecko](https://www.coingecko.com/en/coins/ageur)
* [Eurostable Rankings on CoinGecko](https://www.coingecko.com/en/categories/eur-stablecoin)
