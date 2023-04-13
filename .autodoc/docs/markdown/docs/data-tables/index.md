[View code on GitHub](https://dune.com/docs/data-tables/index.md)

# Tables and Chains Overview

This technical guide provides an overview of the tables and chains available in the Dune app. The guide is divided into two main sections: The Four Kinds of Tables and Available Chains.

The Four Kinds of Tables section explains how Dune ingests data from node providers to create raw tables, which are then decoded using contract ABIs to provide easier to work with decoded tables. Abstracted tables are then created to standardize and aggregate the data, giving users the easiest to work with spell tables. The section also provides links to the raw data, decoded data, spellbook, and community tables.

The Available Chains section provides a list of the chains available to query in Dune. For each chain, the section provides a brief overview of the chain, its history, and its technical details. The section also includes links to the chain's documentation and other resources.

For example, the Ethereum Mainnet section provides a brief history of Ethereum, its updates, and its decentralized platform. The section also includes a link to the Ethereum Developer Docs. Similarly, the BNB Chain (BSC) section explains how BNB Chain follows most of the rules of Ethereum Mainnet but has not implemented EIP1559. The section also includes a link to the BNB Chain Documentation.

Overall, this technical guide provides a comprehensive overview of the tables and chains available in the Dune app. It is a useful resource for users who want to understand how Dune ingests data and creates tables, as well as for users who want to query specific chains and understand their technical details.
## Questions: 
 1. What kind of data can be queried from the Dune Docs app for each available chain?
- The app ingests data from node providers to fill raw tables, which are then decoded using contract ABIs to provide decoded tables. Abstracted tables are then created to standardize and aggregate the data, giving users the easiest to work with spell tables. 

2. How does the gas calculation differ for transactions on Optimism and Arbitrum compared to Ethereum Mainnet?
- Optimism processes transactions outside of Ethereum Mainnet, reducing congestion on the base layer and improving scalability. Arbitrum is an optimistic rollup that settles its transactions on Ethereum Mainnet, but its execution environment differs from the Mainnet EVM implementation in its calculation of gas costs. 

3. What is the difference between BNB Chain and Ethereum Mainnet in terms of gas fees and fee burning?
- BNB Chain follows most of the rules of Ethereum Mainnet, but has not implemented EIP1559. Instead, it relies on BEP-95 to burn fees that accrue during usage of the platform. Furthermore, the gas limit per block is set to 100 million, enabling more transactions to be processed in a given block. Transactions fees are paid in BNB instead of ETH.