# Blockchain Fundamentals

At its core, blockchain is about trust and the ability to conduct transactions without relying on a controlling third party. Key concepts of blockchain include:

## Currency and Cryptocurrency

Currency is based on trust and guarantee of value. Fiat currency is backed by a government or regulatory agency. Cryptocurrency does something similar without the involvement of a third party and is represented digitally. Cryptocurrency also uses cryptography to protect it from manipulation or theft.

## What is Blockchain?

The question of payment raises several concerns including form of payment, can the person being paid accept the form of payment, and more. Blockchain facilities a way to provide payment without worrying about constraints that come with traditional payment methods. Blockchain also provides that ability to view the history of transactions and redundancy of the data through replication and wide distribution over a global network. The blockchain can be public and allow anyone to view transactions.

Data is key to blockchain. Data handling processing traditionally involved creating, reading, updating, and deleting data. Blockchain only supports adding (creating) and reading data. Making updates involving adding an additional record onto the end of the "chain" or ledger of data activity. This process allows the history of the data to be accessible along the entire range of activity from start to the most recent.

The blockchain is in theory, immutable. Data on a blockchain is stored on multiple nodes (servers) which are identical copies. Before changes are allowed, blockchain nodes are compared to verify that there's no differences and if there are, the changes are rejected. A problem emerges when it's not clear which blockchain is correct when comparing two - was a block added or removed? This issue is addressed through consensus of blockchain nodes across at least 3 nodes with the majority of nodes agreeing and verifying which blockchain is correct.

- Data can only be created (added) and read (retrieved)
- Data is immutable
- immutability is established through consensus of the majority of nodes

## Building the Blockchain

A block in the blockchain includes an amount, a source (account), a target (account), and a hash. A hash is a one-way mathematical function that is easy to calculate in one direction but difficult to reverse. For example, a string of characters (ex. 'hello') can be converted to numbers through ASCII codes. To convert 'hello' to ASCII it would be 104 101 108 108 111. A hashing function could add the values up to 532 as the result. Using the number 532 produces an output that is difficult to reverse to produce the same result. A good hash also produces few collisions, which are hashes that produce the same result.

Blocks are chained together beginning with a genesis block (block 0). Adding another block is done by taking the hash of the previous block and adding it to the new block.

The pieces that come together to create an individual block in the blockchain are:

- block number
- current block hash
- previous block hash
- body (transactions)

When one block within the chain is changed, the entire chain is broken since the hashes no longer match.

## Enhancing Security

To prevent creating fake blocks there's a value added to the block data prior to hashing that's called a complexity requirement. Use of a nonce is added to the block data. The nonce is a number that is used to result in a hash that begins with a certain number of zeros. The nonce makes the hash incredibly difficult to fabricate. The process of finding the right nonce is called mining. Bitcoin uses a nonce of 19 leading zeros to create its complexity requirement.

Nodes must all agree on which blocks are allowed to be added to the blockchain, which is called consensus. The process of coming to consensus is called proof of work. The first of miner to find a valid has submits the solution and is validated by other nodes. There are many other types of consensus mechanisms that and be used to validate blocks.

- request submitted to blockchain node
- when node has enough data, it organizes and adds header
- block is submitted for consensus
- if accepted, block is added to chain

## Public vs Private Blockchains

Public (permissionless blockchain) allows anyone to view and participate in the blockchain. Private (permissioned blockchain) allows access to the blockchain to authorized users only.

## Types of Nodes

Full node - downloads full copies of the blockchain.
Lightweight node - participates in the blockchain, but only download the most recent (or needed) blocks.
