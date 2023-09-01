## (Contest Complete) Earn eth finding critical bugs in Ethscriptions Market!

### Results

This competition has concluded! Thanks to all who participated! After reviewing all the submissions and testing the marketplace for more than a month, we have decided that no one was eligible for a prize. However we do appreciate all submissions!

Read below for the original rules.

## Original Announcement

### What is This?

Soon we will be launching a new marketplace on Ethscriptions.com that is based on [ESIP-2](https://ethscriptions.gitbook.io/esips/esip-2-safe-smart-contract-ethscription-escrow-with-transferforpreviousowner).

To help protect everyone's assets, we are holding a **3 ETH BUG COMPETITION** while the marketplace is still on Goerli.

### The Rules

The rules are simple: report a bug that could result in loss of funds or loss of ethscription and you will receive an eth reward!

The exact amount you get will be up to my judgment based on the severity of the bug and the quality of the report. The total amount that can possibly be awarded across all bugs is **3 eth.**

If you find a bug that *wouldn't* lead to loss of funds or loss of ethscription you will not receive a cash reward, but you will receive my eternal gratitude, so you should still consider reporting it!

The bounty ends at 11:59pm EDT on Monday, July 24.

Report bugs by opening issues in this repo.

### Where is the Code?

The marketplace contract is a ERC-1967 proxy [deployed at this address](https://goerli.etherscan.io/address/0xa3eb4cb577d67b0fd5b538ead7376af8e41c8443) that was deployed with the Solady [ERC1967Factory](https://github.com/Vectorized/solady/blob/main/src/utils/ERC1967Factory.sol).

It's unlikely (though not impossible) that you'll find a bug here, so you probably want to focus on the current implementation [which is deployed here](https://goerli.etherscan.io/address/0x6a62d2b1df63673d1c3f4f22af91a703f08a114b#code).

The marketplace logic is in `EthscriptionsMarketV3.sol` and this contract inherits from the `EthscriptionsEscrower.sol` base contract. I copy-pasted both of these contracts from the verified implementation on Etherscan into this repo.

### How can I try it?

The Goerli marketplace is available on https://goerli.ethscriptions.com

### Questions?

DM [@dumbnamenumbers](https://twitter.com/dumbnamenumbers) or [@0xHirsch](https://twitter.com/0xHirsch/) on Twitter. And join the [Ethscriptions Discord](https://discord.gg/ethscriptions)!



