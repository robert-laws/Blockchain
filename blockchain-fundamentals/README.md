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
