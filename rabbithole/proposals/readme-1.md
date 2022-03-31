# Aave - jEUR Listing Supplemental

This is summary of [Aave proposal: Add jEUR on Aave v3 on Polygon (snapshot.org)](https://snapshot.org/#/aave.eth/proposal/0x014370349d306dfd70bb13b81ca299c1d025e177f317de6f910b1a7c70436ce7), submitted 2/25/21 to Aave Governance via Snapshot.org. Written for the RabbitHole Metagovernance Pod by [rathermercurial.eth](https://rathermercurial.eth.xyz).

## AIP: Add jEUR to Aave v3 on Polygon

The Jarvis Network Core Team has proposed the listing of their Euro-pegged stablecoin, $jEUR, on Aave v3 pending its release on Polygon network. Jarvis Network's goal is to provide a new use case to $jEUR as a "Euro savings account on the blockchain".

**Proposed By:** [Jarvis Network Core Team](https://jarvis.network)\
**Start Date:** 2/25/22 | **End Date:** 3/2/22\
**Forum Discussion:** https://governance.aave.com/t/listing-proposal-add-jeur-on-aave-v3-on-polyon/7353\
**Snapshot.Org Vote:** https://snapshot.org/#/aave.eth/proposal/0x014370349d306dfd70bb13b81ca299c1d025e177f317de6f910b1a7c70436ce7

### Risks and Security Considerations

jEUR is overcollateralized by 13% and is backed solely by USDC which received an A- in Aave's own internal risk assessment. Jarvis tokens also inherit risks from UMA's DVM oracle (used to secure liquidations) and the Chainlink EURUSD price feed. Jarvis Network's jFIAT tokens have been audited by [Halborn](https://halborn.com) and [Ubik Group](https://ubikgroup.co).

The minting contract is controlled by a centrally controlled 2/3 multisig, and can delegate certain functions to a "maintainer" multisig such as fee adjustment, adding/removing jFIAT assets and calling an emergency shutdown mode which settles all assets at the Chainlink feed price. Jarvis network is moving to a new governance wallet in 2Q22.

### **Proposed Parameters:**

Jarvis Network has proposed three parameter models for the agEUR market on Polygon: Isolation Mode, v3 Efficiency Mode Stablecoins and a hypothetical "v3 Efficiency Mode EUR Stablecoins", each with varying parameters.

* Reserve Factor: 10-20%
* Base LTV as Collateral: 50-97%
* Liquidation Threshold: 80-98%
* No Specified Liquidation Bonus
* _Borrowing Enabled ✅_
* _Can Be Used as Collateral ✅_

### About Jarvis Network & jEUR

The Jarvis Network's Synthereum protocol issues fiat-pegged synthetic assets (jFIAT) backed by USDC which can be freely exchanged at oracle price (with 0% slippage). Their Euro-pegged stablecoin has been live on Polygon since September 2021.

Combining their efficient fiat on/off ramp (via [Mt Pelerin](https://www.mtpelerin.com)) and unique wrapper for other Euro-pegged assets, Jarvis is uniquely positioned to provide a seamless DeFi/Cefi bridge for users in the European, West African and Central African markets. A listing on Aave would also provide new liquidity markets and arbitrage opportunities to both the Jarvis and Aave ecosystems.

### Important Links:

Jarvis Official Website: https://jarvis.network/\
Jarvis Docs: https://learn.jarvis.network/\
Jarvis Git Repo: https://gitlab.com/jarvis-network\
Jarvis Audits: https://learn.jarvis.network/protocol-overview/security\
Dune Analytics Dashboard: https://dune.xyz/0xroll/JarvisNetwork\
jEUR Token Contract on Etherscan: https://etherscan.io/token/0x0f17bc9a994b87b5225cfb6a2cd4d667adb4f20b\
jEUR Asset Details on CoinGecko: https://www.coingecko.com/en/coins/jarvis-synthetic-euro\
Eurostable Rankings on CoinGecko: https://www.coingecko.com/en/categories/eur-stablecoin
