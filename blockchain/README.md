The content is from LinuxFoundationX LFS170x Blockchain: Understanding Its Uses and Implications. To have the best expirence, please go to edx.org and support Linux foundation
- [**Blockchain component**](#blockchain-component)
  - [**Basic terms of blockchain**](#basic-terms-of-blockchain)
    - [Ethereum](#ethereum)
    - [Smart Contracts](#smart-contracts)
    - [Public Blockchains](#public-blockchains)
    - [Private Blockchains](#private-blockchains)
    - [Digital Wallet](#digital-wallet)
    - [Public Key Infrastructure (PKI)](#public-key-infrastructure-pki)
    - [**In decentralized ledger, it's hard to cheat (51% of copy need to be updated). Event though a node come down, there still other nodes hold the transaction history**.](#in-decentralized-ledger-its-hard-to-cheat-51-of-copy-need-to-be-updated-event-though-a-node-come-down-there-still-other-nodes-hold-the-transaction-history)
  - [**Blockchain = concept of ledger+distributed system**](#blockchain--concept-of-ledgerdistributed-system)
- [**Cryptography and trust**](#cryptography-and-trust)
  - [**Basic term of cryptography**](#basic-term-of-cryptography)
    - [Cryptography](#cryptography)
    - [Secret](#secret)
    - [Key](#key)
    - [Function](#function)
    - [Cipher](#cipher)
    - [Encryption](#encryption)
    - [Decryption](#decryption)
  - [**Byzantine Fault Tolerance -> the idea make blockchain become more secure**](#byzantine-fault-tolerance---the-idea-make-blockchain-become-more-secure)
- [**Types of Cryptography in Blockchain**](#types-of-cryptography-in-blockchain)
    - [Public Key Cryptography](#public-key-cryptography)
    - [Zero-Knowledge Proofs](#zero-knowledge-proofs)
    - [Hash Functions](#hash-functions)
    - [Merkle Trees](#merkle-trees)
  - [**Zero-Knowledge Proofs**](#zero-knowledge-proofs-1)
  - [A comparision of Ethereum vs Hyperledger Fabric](#a-comparision-of-ethereum-vs-hyperledger-fabric)
- [**Blockchain transparency and immutability**](#blockchain-transparency-and-immutability)
- [**Blockchain function**](#blockchain-function)
  - [**Onion model on blockchain:**](#onion-model-on-blockchain)
  - [**Smart contract**:](#smart-contract)
  - [**Blockchain security**](#blockchain-security)
  - [**Different types of blockchain**](#different-types-of-blockchain)
    - [Benefit of public blockchain:](#benefit-of-public-blockchain)
    - [Benefit of private blockchain:](#benefit-of-private-blockchain)
    - [Some point to think of using blockchain or not:](#some-point-to-think-of-using-blockchain-or-not)
  - [**Consensus**](#consensus)
    - [Proof of work:](#proof-of-work)
    - [Proof of stake:](#proof-of-stake)
    - [Bitcoin consensus model:](#bitcoin-consensus-model)
    - [Etherum consensus model:](#etherum-consensus-model)
    - [Hyperledger Fabric Consensus Model:](#hyperledger-fabric-consensus-model)
    - [Corda Consensus model:](#corda-consensus-model)
  - [**Blockchain and gorvernance**](#blockchain-and-gorvernance)
    - [On-chain vs off-chain gorvernance](#on-chain-vs-off-chain-gorvernance)
  - [Blockchain gorvernance stategry:](#blockchain-gorvernance-stategry)
  - [Advanced blockchain anonymity techniques:](#advanced-blockchain-anonymity-techniques)
  - [Some case study of advanced anomyty techniques:](#some-case-study-of-advanced-anomyty-techniques)
  - [Trust in blockchain](#trust-in-blockchain)
  - [Blockchain Immutability Concept](#blockchain-immutability-concept)

# **Blockchain component**

- Ledger (associate with accountant) - a collection of transaction. In blockchain, the ledger is distributed (or decentralize) -> no one/ everyone own the ledger.
- A transaction is compose of sender, receiver and the assets
- Some of blockchain implementation have smart contract. Smart contract is rule to make transaction of block chain.
- There are public blockchain and private blockchain.
- In blockchain network, there are nodes. Each nodes have the copy of ledger
- Private blockchain have the authorization/authentication service (aka membership service provider)
- Have identity of user, achieved by PKI provide public key -> identity of the user on the network. And the private key store in wallet (**wallet is a collection of the user credentials**)
- People interact with blockchain through **event**

## **Basic terms of blockchain**
### Ethereum
- Ethereum, like Bitcoin, is a decentralized open-source blockchain. Unlike the Bitcoin Network, the Ethereum Protocol has the ability to run smart contracts. The cryptocurrency running on the Ethereum network is called Ether.
### Smart Contracts
- A smart contract is computer code that can be run on a blockchain that executes the conditions of an agreement.
### Public Blockchains
- Public blockchain has no barrier to entry. Anyone with a cell phone and a digital wallet can transact on the blockchain.
### Private Blockchains
- Private blockchains or permissioned blockchains have a Membership Services piece that grants access to users before they can interact with the blockchain.
### Digital Wallet
- A digital wallet is a computer application that represents a traditional wallet. It gives the user the ability to store and transact cryptocurrencies through the Internet.
### Public Key Infrastructure (PKI)
- Public Key Infrastructure is the identity management system for instilling trust into the electronic transfers of information or value. It is the technology used to authenticate users and information by issuing a set of key pairs (public and private).

### **In decentralized ledger, it's hard to cheat (51% of copy need to be updated). Event though a node come down, there still other nodes hold the transaction history**.

## **Blockchain = concept of ledger+distributed system**

<br>

# **Cryptography and trust**

## **Basic term of cryptography**
### Cryptography
- Cryptography is a technique used to secure the communication between two parties from a third. The term cryptography is derived from two ancient greek terms, “kryptos” which means “hidden” and “graphein” which means “to write”.
### Secret
- The data which we are trying to protect.
### Key
- A piece of data used for encrypting and decrypting the secret.
### Function
- The process or function used to encrypt the secret.
### Cipher
- The encrypted secret data, the digital secret, the output of the mathematical function or a cryptographic algorithm.
### Encryption
- This is the process from plain text (ordinary text) to cipher text (random sequence of bits).
### Decryption
- Encryption is the reverse process of converting ciphertext into plain text.
<br> 

**One of the technologies that plays a pivotal role in blockchain and making blockchain secure and immutable is cryptography.**

## **Byzantine Fault Tolerance -> the idea make blockchain become more secure**

<br>

# **Types of Cryptography in Blockchain**

### Public Key Cryptography
- This encryption method uses a pair of keys: an encryption key, and a decryption key, named public key and private key, respectively. The key pair generated by this algorithm consists of a private key and a unique public key that is generated using the same algorithm.
### Zero-Knowledge Proofs
- A new approach to protecting digital secrets that prove knowledge of a secret without revealing it.
### Hash Functions
- This type of encryption doesn’t make use of keys. It uses a cipher to generate a hash value of a fixed length. The function converts plain text (no matter the size) into a hash of fixed size. It is nearly impossible for the contents of plain text to be recovered from the cipher text. Think of it like trying to recreate a human from a fingerprint, a fingerprint uniquely represents a human no matter the size of the human and you can’t reverse engineer a fingerprint to recreate the human.
### Merkle Trees
- A data storage technique that compresses or packs data for storing blockchains with a tamper-free component built in. Merkle trees are built upon hashing principles in that each hash becomes a part of the next hash to build a tamper resistant data storage model.


## **Zero-Knowledge Proofs** 
- https://appinventiv.com/blog/zero-knowledge-proof-blockchain/

## A comparision of Ethereum vs Hyperledger Fabric

The use of public keys for identity management is a logical choice since knowledge of a public key is necessary for verification of digital signatures. Both Ethereum and Hyperledger Fabric use digital signatures on transactions and blocks to verify the identity of the creator and that the signed data has not been modified since signing. Public key cryptography is used in the blockchain as a method for managing users’ identities without revealing real world identities.

In Ethereum, users are identified by an address that is directly related to the user's public key. This provides identity verification while preserving anonymity.

In Hyperledger Fabric, users are identified via X.509 certificates. These certificates provide several pieces of information about the user, but one of these is also the user's public key.

Hash functions are at the core of all blockchain technology. One of the primary uses for hash functions is chaining blocks together. In both Ethereum and Hyperledger Fabric, blocks include the hash of the previous block to tie the blockchain into a cohesive whole.

Zero-knowledge proofs are to increase the privacy of users. Currently, Ethereum is working on a layer 2 solution, where a second layer blockchain would store large amounts of data and only prove the batch of information is valid to layer 1 (mainnet). Hyperledger Fabric has a pluggable cryptographic library that supports ZKP techniques for enhanced privacy measures.

Merkle trees are a data structure that allows authenticated storage with efficient data retrieval. Both Ethereum and Hyperledger Fabric are smart contract platforms that use a particular type of Merkle tree called the Patricia tree to store the current state of their virtual machine.


# **Blockchain transparency and immutability**

The blockchain is designed to be a data structure that only allows appending -> The past history of the blockchain is visible and immutable.
- Updates to the blockchain can be performed by including them in new blocks added to the blockchain.
- The blockchain is designed as a data structure where each block in the chain locks in the value of the previous block and so on, back to the first or genesis block. This means that the blockchain is an append-only data structure without support for modification or deletion.

- **The entire history of the blockchain is publicly visible and stored in a distributed and decentralized fashion**. Values in the blockchain can be “updated” by appending a new version of that value in a later block, but the complete history of the value is preserved.
- **Transactions** in the blockchain cannot be modified after creation, and their complete history is publicly visible. This means that the blockchain is a completely transparent data structure with the useful property that the integrity of the blockchain is easily verifiable (by cryptography algorithm) by any user.
- **Immutability in the Blockchain Is Essential.** This is achieved by these techniques:
  - At the bottom level, transactions are digitally signed by their creators. An attacker can’t forge a transaction unless they steal a private key.
  - A block structure is predefined. Attackers can’t modify it to suit their purposes.
  - The chain part of the blockchain is achieved using hash functions. Each block includes the hash of the previous block, creating a clear link between each block in the blockchain.
  - Each block is digitally signed by its creator. The creator is selected through the blockchain’s consensus protocol, making it difficult for an attacker to be a legitimate creator. The creator of a block is either publicly known (Proof of Stake) or difficult to become (Proof of Work), making masquerading as the real creator difficult or impossible.


# **Blockchain function**
## **Onion model on blockchain:**
- Two or more parties coming together and using the blockchain to record an announcement of the exchange of monetary value. (first layer - first type of transaction)
- Two or more parties using blockchain to record an important announcement. (second layer - second type of transaction)
- A single party announcing an important or significant event. (third layer - third type of transaction)
## **Smart contract**:  
- And smart contracts are just computer code. They're codified logic that we can use to respond to any kind of event that gets captured on the blockchain.
These are some of the features that smart contracts provide:

- These are some of the features that smart contracts provide:
  - Accuracy: Replacing human intermediaries with executable code ensures the process will always be performed the same.
  - Cost savings: Replacing intermediaries often provides significant cost reduction.
  - Efficiency: Removing process intermediaries often results in significant process efficiency gains.
  - Backup: A blockchain and smart contract deployed to it can provide a permanent record, allowing for auditing, insight, and traceability, even if the creator is no longer in business.
  - Autonomy: Smart contracts can be developed by anyone, no need for intermediaries such as lawyers, brokers, or auditors.

<br>

## **Blockchain security**

Difference terms Standard Cyber security vs Blockchain Cyber security

| Standar cyber security                                                                                                                                                                                                                                                                    | Blockchain cyber security                                                                                                                                                                                                                                                                                                      |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| The traditional computing environment is a company network fully or, at least mostly, under the control of the company's computer security staff.                                                                                                                                         | Blockchains are designed to be decentralized, distributed systems running on untrusted hardware.                                                                                                                                                                                                                               |
| While many organizations are making the shift to cloud-based environments, they still have a high degree of control over the security and configuration of their rented systems.                                                                                                          | While security in traditional environments is designed to provide security by putting all data in one place and building walls around it, security in blockchain is based on ensuring that data is protected from modification by copying data to as many locations as possible to make modification of all copies infeasible. |
| Traditional networks are highly centralized, and the focus of cybersecurity on these systems is primarily perimeter-focused. All systems and authorized users on the network are trusted or semi-trusted, so the focus is on preventing attackers from entering from outside the network. | Traditional infrastructure focuses on confidentiality and integrity, while blockchain is designed to provide integrity and availability.                                                                                                                                                                                       |

<br>
<br>

## **Different types of blockchain**
When we try to understand the main difference between a public and private blockchain, it is important to understand the terminology:

- **Public Blockchains**:  A public blockchain is open to anyone to join. Public blockchains are decentralized where no one has control over the network. These immutable and censorship resistant networks are ideal for participants who don't trust each other, but still interact in a network and take part in consensus. Bitcoin and Ethereum are examples of public, permissionless blockchains.
- **Permissionless Blockchains**: Public blockchains are permissionless. Anyone effectively can join the blockchain network. No one is prohibited from joining.
- **Private Blockchains**: Private blockchains define a user's rights on the network prior to admittance. Restrictions are placed on activities such as who can write to the ledger and what transaction they can participate in. Hyperledger and Corda blockchains are examples of private permissioned blockchains.
- **Permissioned Blockchains**: In a permissioned blockchain, participation is permissioned by an organization or a consortium of organizations. This empowered entity defines who can participate in certain transactions and consensus on the network.

<br>

### Benefit of public blockchain:
- **Ledger is distributed**: The database is not centralized like in a client-server approach, and all nodes in the blockchain participate in the transaction validation.
- **Immutable**: When something is written to the blockchain, it cannot be changed.
- **Open Consensus Model**: No restriction placed on who can operate a node in the network.
- **Open read and write**: Anyone can participate by submitting transactions to the blockchain, such as Ethereum or Bitcoin; transactions can be viewed on the blockchain explorer.
- **Low barrier to entry**: Transactions on a public network can be accomplished with an Internet connection and a cell phone.
- **Secure due to mining (51% rule)**: With Bitcoin, obtaining a majority of network power could potentially enable massive double spending, and the ability to prevent transaction confirmations, among other potentially nefarious acts. This has never been accomplished as the computing power needed to stage such an attack would be too costly.

<br>

### Benefit of private blockchain:
- **Ledger is distributed/immutable**: The database is not centralized like in a client-server approach, and all nodes in the blockchain participate in the transaction validation. When something is written to the blockchain, it cannot be changed.
- **Compliance support**: As an enterprise, you likely would have compliance requirements to adhere to, and having control of your infrastructure would enable this requirement more seamlessly.
- **Faster transactions**: When you distribute the nodes locally, but also have much less nodes to participate in the ledger, the performance is faster.
- **Consensus more efficient/more options**: More options for consensus models. Enterprise or private blockchains have less nodes and usually have a different consensus algorithm, such as BFT vs. POW.
- **Better scalability**: Being able to add nodes and services on demand can provide a great advantage to the enterprise.
- **Enterprise permissioned**:  The enterprise controls the resources and access to the blockchain, hence private and/or permissioned.

<br>

### Some point to think of using blockchain or not:
- **Blockchain decisions**: When it comes to decision making around which blockchain model to use, it's important to determine which platform and structure is right for your business.
- **Intermediaries**: Blockchain implementations can eliminate middlemen from work processes.
- **Central authority** Some organizations rely on one person having control, with blockchain decentralized work flows without a single point of failure are emerging.
- **Multi-party interaction**: Blockchain provides a trust layer that opens up new opportunities for participation.
- **Visibility**: Blockchain transparency reduces dispute over what is in the ledger since agreement occurs before transactions are committed and everyone can have access to the ledger.
- **Write access**: Public permissionless blockchains do not prohibit who can add blocks to the chain, where private permissioned can restrict access.
- **Value transfer**: Blockchains can differ in the ways participants transfer value.

## **Consensus**

### Proof of work:
In Proof of Work, users in the blockchain network who want to create the next block (and win the associated reward) are called miners. To win the right to mine a block, miners race to find an acceptable solution to a “hard” cryptographic problem. (...), “hard” mathematical problems can only be solved by random guessing. When a miner finds an acceptable solution, they create a block and broadcast it to the network, finalizing that block.

Proof of Work exploits the scarcity of computational resources by choosing a problem that can only be solved by guessing. There is no limit on the number of guesses that a miner can make at once. Proof of Work, therefore, incentivizes miners to run as many mining machines as possible to maximize the probability that they are the first to find a solution to the problem. Since mining computers take money to purchase and money to run, the amount of control that a user can exert over the blockchain is limited by the amount of money they have available to invest in mining equipment.

The security of the Proof of Work consensus is based on the assumption that no one controls more than half of the computational resources of a blockchain’s mining network. If one entity controls 51% of the mining effort, they control consensus. To take control would require a huge investment in equipment and energy, more than would be gained by defrauding the system.

### Proof of stake:
Proof of Stake comes with a number of improvements to Proof of Work systems, it requires less energy and has a lower barrier to entry since no specialized hardware is required to create blocks.

Users in a Proof of Stake blockchain can "stake" or promise not to use the tokens they own. This gives them the opportunity to be selected as the next user to create or "forge" a new block and earn the reward. A block forger is pseudo-randomly selected from all of the users who have staked some of their assets, and the selection process is biased based on the size of the stake.

For example, imagine that a wheel is divided into sections where the size of a section is proportional to the size of a user’s stake. The next block creator would be chosen by spinning the wheel and seeing whose section comes out on top. In Proof of Stake, each user has a copy of the wheel and they are all synchronized so that each person can independently determine the selection and get the same result. This is why Proof of Stake uses a pseudo-random instead of a random selection process.

In Proof of Stake, an attacker needs to control enough of the staked currency to guarantee they will be selected to create every block. Since cryptocurrency is a limited asset, buying up enough of it to do this is expensive, making attacks on Proof of Stake systems economically infeasible.

### Bitcoin consensus model:

Bitcoin, the first blockchain to appear, uses Proof of Work which requires miners to solve a complex cryptographic mathematical puzzle for which they get rewarded. Block rewards are newly minted Bitcoin granted to the miners that solve the puzzle first. Built into the Bitcoin blockchain protocol, is an event called halving. Bitcoin halving happens every four years and Bitcoin’s block reward gets cut in half. The halving occurs when the block height reaches a certain point (210,000 blocks) which is programmed into the protocol. The first halving occurred in November 2012 and the block reward was cut from 50 BTC to 25 BTC. The second occurred July 9, 2016 and the reward was reduced to 12.5 BTC. The third occurred on May 11th 2020, cutting the block reward to 6.25. The next halving is estimated in the year 2024 and the reward will be reduced to 3.125 BTC. The Bitcoin network is programmed to produce only 21 million bitcoin and the halving is what keeps inflation in check by slowing down the distribution. About ⅔ of the 21 million BTC have been mined so far.

### Etherum consensus model:

Ethereum currently uses Proof of Work for a consensus model. Ethereum was introduced in a white paper by Vitaly Dmitriyevich "Vitalik" Buterin, a Russian-Canadian entrepreneur and programmer from Toronto. He envisioned the second-largest cryptocurrency when he “forked” or copied the Bitcoin code, made improvements and created the Ethereum blockchain. This new blockchain was not only a currency exchange system but along with the Ethereum Virtual Machine, an interconnect, turing complete computer, open to programmers to develop. It creates a platform that smart contracts can be executed and applications can be built upon. Ethereum has always planned to move away from a Proof of Work consensus mechanism to a Proof of Stake. Plans for Ethereum to adopt Proof of Stake will occur when Ethereum 2.0 is incorporated, this improvement is expected sometime in the second half of 2021.

### Hyperledger Fabric Consensus Model:
Hyperledger Fabric is a private permissioned blockchain platform that breaks consensus into components, allowing users to pick a consensus algorithm for their particular situation. Instead of a predetermined consensus model, Hyperledger has an ordering service that performs consensus related events, this ordering component can pick the consensus model that best suits the blockchains needs. By approaching consensus in this modular fashion, Hyperledger DLT’s can change consensus models without huge overhauls to the code base.

As explained by Demiro Massessi,

"Hyperledger Fabric deliberately avoided hard-coding a consensus mechanism into the protocol by defining an “orderer component” that performs all of the consensus-related operations. This allows users of Hyperledger Fabric to select a consensus algorithm that fits their use case without being forced to make large-scale code edits".

### Corda Consensus model:

Corda is a private permissioned blockchain. Each Corda network has a notary service made up of independent parties that approve blocks using any applicable consensus algorithms.

As mentioned in Jamiel Sheikh's book “Mastering Corda: Blockchain for Java Developers”, R3 provides a set of Corda applications called The Corda Business Network Toolkit to manage one or more Corda networks. Corda does not follow the standard blockchain model of transactions being bundled into blocks and then being finalized by the network as a whole. Instead, a Corda network contains one or more notaries consisting of several independent parties. Transactions in Corda are finalized by a notary with a multiparty digital signature using an algorithm like Raft.

## **Blockchain and gorvernance**

### On-chain vs off-chain gorvernance 
- **On-chain gorvernance**: In the on-chain governance, rules for instituting changes are encoded into the blockchain protocol. This means that any decision being made is automatically being translated into code (e.g. decisions concerning block size). Developers propose changes through code updates and each node votes on whether to accept or reject the proposed change.
- **Off-chain gorvernance**: Off-chain governance can be seen as decision-making that first takes place on a social level and is later actively encoded into the protocol by the developers. For instance, Bitcoin developers share their improvement proposals (BIPs) through a mailing list, whereas Ethereum collects improvement protocols (EIPs) on GitHub.

## Blockchain gorvernance stategry:
- Benevolent dictator for life: The original creator or lead developer of a cryptocurrency has the final say on all decisions. The simplest governance strategy is nicknamed benevolent dictator for life. In this strategy, the creator of the blockchain is the final authority on all decisions regarding the blockchain (...).
- Core development team: A team of the most active developers decides what functionality should or shouldn’t be included. The next step up places control of the blockchain roadmap in the hands of a core development team. This is a strategy commonly used in open source programming projects, where users are able to offer or request features, but developers have the final say on what is or is not included in the official release.
- Open governance: The team making governance decisions for the blockchain is chosen by the users of the blockchain. Some blockchains use the open governance method of handling governance of the blockchain. In this system, the team that makes the final technical decisions for a system is selected by the system’s users.
- On-chain governance: The rules for how the blockchain operates are stored on-chain in smart contracts with built-in capability and procedures for modifications. A blockchain-specific governance strategy is on-chain governance. In this form of blockchain governance, the rules describing how the blockchain should operate are stored on the blockchain itself. These regulations typically are implemented as smart contracts on the blockchain with built-in methods for users to modify the rules based upon their needs and the needs of the blockchain".

## Advanced blockchain anonymity techniques:
- **Zero-knowledge proofs**: Zero-knowledge proofs use cryptographic algorithms to allow a user to prove knowledge of a secret without revealing the secret. A prover proves knowledge of a secret without revealing it. New technology referred to as SNARK (Succinct Non-interactive - ARgument of Knowledge) are fine tuning privacy issues on blockchains.
- **Stealth addresses**: Stealth addresses involve using one-time addresses to perform transactions on a blockchain. A stealth address is just a one-time address that makes it impossible to link a transaction to a known account. This prevents the data mining attacks on privacy that we discussed earlier.
- **Ring signatures**: We mentioned previously that transactions are digitally signed. With ring signatures, all that can be determined from a transaction is that a member of a group signed it, but not the particular member.
- **CoinJoin** The ability to see who is performing transactions with whom is dangerous to user privacy and anonymity. Protocols like CoinJoin mix several transactions together so that it is difficult to pair senders with recipients.
- **Confidential transactions**: Confidential transactions take advantage of homomorphic encryption, which makes it possible to perform mathematical operations on encrypted data. This means that the data contained in a transaction can be hidden from the public, while still allowing the network to verify that the transaction is valid.

## Some case study of advanced anomyty techniques:
- ### **Ethereum**: 
  - Ethereum is working on improving the zero-knowledge proofs, mixing and DAPPS (applications developed to improve anonymity) to strengthen privacy. Also ConsenSys, the Enterprise Solutions builder for Ethereum introduced QUORUM, a fork of the Ethereum blockchain which enables users to benefit from the public Ethereum blockchain while enjoying features from a private network. Developed by JPMorgan, it is a permissioned implementation.
- ### **Hyperledger**:
  - Channels: Subsections of the blockchain that make transactions visible only to members.
  - Private transactions: Hashes of private data are stored to publicly verify it on the blockchain.
  - Zero-knowledge technology: One can demonstrate knowledge of a secret without revealing the secret itself.
- ### **Hyperledger Besu**:
  - Besu is an Ethereum client that runs on the Ethereum public network, private networks, and test networks such as Rinkeby, Ropsten, and Görli. Hyperledger Besu includes several consensus algorithms including PoW, PoA, and IBFT, and has comprehensive permissioning schemes designed specifically for uses in a consortium environment.
- ### **Corda**:
  - Parties on the Corda Network can be represented in one of two ways:
    - Party: A public key and name.
    - Anonymous party: Only a public key.

## Trust in blockchain
Just as there are benefits with blockchain technology, there are also some challenges. Blockchain is a culmination of technologies that have been blended to provide a trustless platform. Expect some challenges and use case justifications taking the old line of business apps to the blockchain.

Let's recap the features of a blockchain that establishes trust:

- Blockchain technology is about storing some kind of data (which are transactions in regards to the Bitcoin blockchain).
- Blockchain is essentially transferring trust from an intermediary to technology.
- Storing data in the blockchain is through cryptographic functions.
- Private key/public key.
- Collaboration through consensus.

## Blockchain Immutability Concept
There are many different variables, but the main one is consensus. In a blockchain, it refers to the logs of transactions which are created by consensus among the chain’s participants. The basic notion is that once a blockchain transaction has received a sufficient level of validation and posted on the chain, it can almost never be replaced, reversed or edited.

If someone wanted to undermine the immutability of the Bitcoin blockchain, here’s how they would do it:

- First, they would install more mining capacity than the rest of the network put together, creating a so-called “51% attack”.
- Second, instead of openly participating in the mining process, they would mine their own “secret branch", containing whichever transactions they approve and censoring the rest.
- Finally, when the desired amount of time has passed, they would anonymously broadcast their secret branch to the network.

<br>

Since the attacker has more mining power than the rest of the network, their branch will contain more Proof of Work than the public one. Every Bitcoin node will therefore switch over since the rules of Bitcoin state that the more difficult branch wins. Any previously confirmed transactions not in the secret branch will be reversed and the Bitcoin they spent could be sent elsewhere. The computing power required to achieve this is enormous and probably only theoretical, but it’s important to consider.

<br>

One other less technical and malicious example would be from the Ethereum hard fork that directly happened after the DAO hack. In this example, the majority of the Ethereum nodes in the network decided to update the software preventing those hackers from withdrawing the cryptocurrency “earned” (stolen). This update could not be enforced, since every Ethereum user controls their own computer. Nonetheless, it was publicly supported by Vitalik Buterin, Ethereum’s founder, as well as many other community leaders. As a result, most users complied, and the blockchain with the new rules kept the name "Ethereum". A minority disagreed with the change and continued the blockchain according to its original rules, earning the title "Ethereum Classic".