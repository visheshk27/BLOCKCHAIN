# BLOCKCHAIN
DEFINATION+GLOSSARY

Blockchain is a system of recording information in a way that makes it difficult or impossible to change, hack, or cheat the system.

A blockchain is essentially a digital ledger of transactions that is duplicated and distributed across the entire network of computer systems on the blockchain. Each block in the chain contains a number of transactions, and every time a new transaction occurs on the blockchain, a record of that transaction is added to every participant’s ledger. The decentralised database managed by multiple participants is known as Distributed Ledger Technology (DLT).

Blockchain is a type of DLT in which transactions are recorded with an immutable cryptographic signature called a hash.

Objective :
visualizing bitcoin blockchain and discussing how exactly bitcoin uses blockchain


Types of Blockchains:
There are basically three types of Block chains:

Public Blockchains
Permissioned Blockchains
Private Blockchains
The terms public, permissioned, and private refer to who has the ability to be a user of, or run a node on the Blockchain. Each type of Blockchain places a different level of importance on anonymity, immutability, efficiency, and transparency.

Public Blockchain
On a public Blockchain anyone can be a user or run a node. Public Blockchains such as Bitcoin value anonymity, immutability, and transparency over efficiency.

Permissioned Blockchain
Permissioned Blockchains are operated by known entities such as stakeholders of a given industry. They value immutability and efficiency over anonymity and transparency. The Financial industry would use such a Blockchain to reduce the time of international payments from days to seconds.

Private Blockchain
Private Blockchains are operated by one entity. These Blockchains value efficiency over anonymity, immutability and transparency. Their use cases are limited.


Glossary :

Bitcoin :
Bitcoin is a digital currency (also called crypto-currency).

According to Wikipedia:

Bitcoin is a cryptocurrency and worldwide payment system. It is the first decentralized digital currency, as the system works without a >central bank or single administrator. The network is peer-to-peer and transactions take place between users directly, without an >intermediary. These transactions are verified by network nodes through the use of cryptography and recorded in a public distributed >ledger called a blockchain


Block
Blocks are files where transactions are permanently recorded. A block records some or all of the most recent Bitcoin transactions that have not yet entered any prior blocks. Thus a block is like a page of a ledger or record book. Each time a block is ‘completed’, it gives way to the next block in the blockchain. A block is thus a permanent store of records which, once written, cannot be altered or removed.

Contents of a Block
Block # :
It is a number which behaves like a counter. Every new block mined is given a Block # which is one greater than its previous block. The Block # starts from 0.Also called depth of a block in the Bitcoin Blockchain. Count of current number of blocks can be seen here.

Block Structure :
Field	Description	Size
Magic no	value always 0xD9B4BEF9	4 bytes
Blocksize	number of bytes following up to end of block	4 bytes
Blockheader	consists of 6 items	80 bytes
Transaction counter	positive integer VI = VarInt	1 - 9 bytes
Transactions	the (non empty) list of transactions	many transactions
Number of Transactions:
The absolute limit is the size of the block, which is currently hard-coded at 1,000,000 bytes. Each transaction takes up a variable amount of space, but ~250 bytes is about right for a simple transaction.

However as soon as a block is mined it is not possible to extend the block by adding in more transactions, as the proof of work has to be redone, so broadcasting it immediately is the only sensible thing to do. So the number of transactions in a block is actually a function of the number of transactions being generated over a time period and the time taken to solve a given block.

Height:
The number of blocks preceding a particular block on a block chain. For example, the genesis block has a height of zero because zero block preceded it.

Block Reward:
Every block also contains a record of which Bitcoin addresses or scripts are entitled to receive the reward. This record is known as a generation transaction, or a coinbase transaction, and is always the first transaction appearing in every block. The number of Bitcoins generated per block starts at 50 and is halved every 210,000 blocks. Bitcoin transactions are broadcast to the network by the sender, and all peers trying to solve blocks collect the transaction records and add them to the block they are working to solve. Miners get incentive to include transactions in their blocks because of attached transaction fees.

Timestamp:
A node adds a timestamp as soon as it detects a new block in the network. So, it can be said that the timestamp is a rough indicator of when the block was formed by the miner. It is possible that the timestamp of a newer block is older that the timestamp of the older block.

From bitcoin.it/wiki/Block_timestamp:

A timestamp is accepted as valid if it is greater than the median timestamp of previous 11 blocks, and less than the network-adjusted >time + 2 hours.

Mined by:
Name of the miner or the mining pool which mined the block. Blocks do not need to contain any identifying factors. The miner can choose to provide a script in the coinbase of a new block that can be used to identify the source of the block, however they are not required to do so. Hence, some blocks have empty 'Mined By' field.

Merkle Root:
It is the hash of the root node of the particular block's Merkle Tree. For more information see Merkle Tree.

Previous Block:
The block preceeding the current block is known as the previous block. Each block is guaranteed to come after the previous block chronologically because the previous block's hash would otherwise not be known. Because a block can only reference one previous block, it is impossible for two forked chains to merge.

Difficulty:
The difficulty of the mathematical problem is automatically adjusted by the network, such that it targets a goal of solving an average of 6 blocks per hour. Every 2016 blocks (solved in about two weeks), all Bitcoin clients compare the actual number created with this goal and modify the target by the percentage that it varied. The network comes to a consensus and automatically increases (or decreases) the difficulty of generating blocks.

Bits:
Size(bytes):
There was no limit on the size of Bitcoin originally but a limit of 1 MB was set later because of problem of Denial of Service Attack. Denial of Service attack is basically huge blocks of transactions which are not possible to process with current technology. The Bitcoin community is divided on this issue as some of them say that the block size must be increased in order to make Bitcoin competitive with other currency mediums such as Paypal while others argue that it must be kept constant so that there is less difficulty in mining the block.
@crackingfactory <3
