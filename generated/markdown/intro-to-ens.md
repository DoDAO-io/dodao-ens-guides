## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

---

## Intro to ENS


## Overview

Ethereum name service(ENS) is a decentralized naming protocol that maps the human-readable addresses to the cryptographic addresses 
or Ethereum addresses on the Ethereum mainnet. It works similarly to DNS, where DNS maps the domain to the IP addresses but has a significantly different 
architecture due to the capabilities and constraints provided by the Ethereum blockchain.

Just like DNS, ENS also uses dot-separated hierarchical domain names. The owner of a domain has complete control over its subdomains. So, if a user owns alice.eth, 
that user can also create pay.alice.eth or mail.alice.eth, and so on. ENS makes it easy for users to create these subdomains from the main domain.
Users can set subdomains without any limit and users have access to assign new owners for the domains and sub domains.

An ENS domain with an .eth TLD (top-level domain) is an NFT. So, it can be traded like an NFT in marketplaces like Open Sea. For example, Alice.eth is an NFT, but Alice.xyz is not an NFT.
ENS domains are a great way to manage multiple web services in one easy-to-use, decentralized address. The following records can be added to the ENS domains
* ETH/BTC/Doge/LTC/Atom/Dash +40 other wallet addresses.
* IPFS content hashes.
* Custom text records
* Keywords
* URLs
* Github handles
* Twitter handles
* Email addresses
* Avatars
* Telegram and reddit handles


    


---
## Evaluation





##### What is ENS?  

- [ ]  ENS is a centralized entity which helps for hosting the websites
- [x]  ENS is a decentralized naming protocol that maps the human-readable addresses to the cryptographic addresses
- [ ]  ENS is a DeFi protocol for lending and borrowing
- [ ]  ENS is a protocol for testing smart-contracts





##### Which of the following is correct about ENS domains?  

- [x]  ENS domains with .eth top level domain is an NFT
- [x]  ENS maps human-readable names to cryptographic addresses
- [ ]  Subdomains cannot be created using ENS domains
- [ ]  ENS Domains can be used only for URLs

    


---
## Advantages of ENS


### Advantages of ENS over DNS 

**Security and decentralization:**
The security is very high in ENS when compared to DNS. The domains are secured by the Ethereum blockchain. ENS is decentralized so there is no censorship resistance and The protocol is transparent.

**Efficiency and Simplicity:**
ENS simplifies the transactions of the cryptocurrency. We can register our owned DNS domains in ENS. ENS domains can have multiple use cases example, they can be used for payments, web 
domains(can be used for multiple websites), Twitter handles, email addresses, etc. The domain names can have emojis in ENS. Users are allowed to create multiple subdomains with single ENS domain. 

### Difference between ENS and DNS

| ENS                                                                                                                                                          | DNS                                                                             |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------- |
| ENS maps human-readable domains to Ethereum addresses or cryptographic addresses.ENS domains can be used instead of wallet address,twitter handles,URL, etc. | DNS maps human-readable domains to IP addresses.DNS domains can be used for URL |
| In the case of ENS, the domains are verified by multiple nodes or computers                                                                                  | In the case of DNS, the verification is centralized                             |
| The domain names are secured by the Ethereum blockchain                                                                                                      | The domain names are stored by centralized authority                            |
| ENS allows users to register with the owned DNS domain                                                                                                       | DNS doesn't allow ENS domains to register                                       |
| ENS is a bit slower comparatively                                                                                                                            | DNS is faster when compared to DNS                                              |
| ENS is resistant to censorship                                                                                                                               | DNS allows censorship as it is centralized                                      |


    


---
## Evaluation





##### How the ENS domains are secured?  

- [ ]  The ENS domains are secured by the centralized server
- [ ]  They are secured by strong security system which can accessed by only 10 centralized entities.
- [x]  The ENS domains are secured by the Ethereum blockchain
- [ ]  They are not secured





##### what are the advantages of ENS domains by being decentralized?  

- [x]  High Security provided by Ethereum blockchain
- [x]  Resistance to censorship
- [ ]  Domains are free
- [ ]  Users gets incentives on purchasing the domains





##### Which of the following are correct?  

- [ ]  ENS and DNS both are centralized
- [x]  Security in ENS is better than DNS.
- [x]  Users are allowed to create multiple subdomains with one ENS domain.
- [x]  ENS domains can be used for various purposes like wallet address, twiiter handles, etc.

    


---
## Important contracts

ENS contains two main smart contracts which are responsible for the working of the ENS domains. They are registry and resolver. The registry contract contains all the necessary 
information like the owner address of the domain, the address of the resolver contract, etc. The resolver contract manages the queries for example if an user wants to associate url or email with the ENS domain resolver will associate the text records to the domain. Resolver maps ENS names to addresses.

### Registry 
This is the smart contract that stores all the domains and subdomains with the following records.
1. Address of the owner
2. Address of resolver contract
3. TTL(Time-to-live) the time period for the expiration of the domain.

All the records are stored in Record(struct data type). The domain names are mapped as hashes using namehash algorithm and called nodes. The nodes are mapped to the Record, which 
contains the addresses of the owner, the resolver contract, and the Time-to-live value. The domains are not directly stored in registry. Instead, they are stored as hashes. Hashes are 
excellent for providing a fixed-length identifier that can be passed around easily between contracts. Before being hashed with namehash, names are first normalized using a process called UTS-46 normalization.
The output of the namehash is called “Node.”

### Resolver 
Resolvers are responsible for translating the name to the addresses or other data provided by the user. Resolving a name in ENS is a two-step process: First, ask the registry what resolver is responsible for the name,
and second, ask that resolver for the answer to your query. A resolver can be any contract that meets the relevant standards to act as a resolver. For example according to EIP-137 the resolver contract must have the function.
```
supportsInterface(bytes4 interfaceID) constant returns (bool);


    


---
## Evaluation





##### what is Registry?  

- [ ]  Registry is a smart-contract which translates names to addresses and to other data.
- [x]  It is the smart contract that stores all the domains and subdomains with addresses of owner, resolver and TTL.
- [ ]  Registry is a smartcontract which can be used for purchasing domains in ENS
- [ ]  Registry is a smart-contract which is used for trading ENS domains as NFT





##### Which of the following is correct about resolver?  

- [x]  Resolver is a contract which translates names to addresses and other data provided by the user
- [x]  It is responsible for managing queries like associating the text records provided by user to the ENS domains
- [ ]  It is responsible for storing the domains and addresses
- [x]  A smartcontract contract can be a resolver That meets relevant conditions for being. Users can create their own resolver





##### What is node in ENS?  

- [x]  Node is the output of namehash algorithm with the name as input
- [ ]  Node is an another smart-contract which stores the domains and addresses for backup
- [ ]  Node is an algorithm which is used for hashing the names of ENS domains
- [ ]  None of these

    


---
## Working

### Working 

Users can buy an available domain, after buying the domain user must set up the addresses for the wallet and resolver. User can set a public resolver or a custom resolver. Name is hashed and recorded in the registry, 
along with their node's address, resolver address, and TTL. The nodes are mapped to the record, which has the owner’s address, resolver address, and TTL. We need to assign the resolver after owning the domain successfully. 
We can set up a public resolver that has most of the necessary functionalities. However, users can also create and use their own custom resolvers according to their specific needs. Users are also required to setup reverse 
records for replacing of addresses with domain names such that names are displayed instead of addresses.

Resolving a name in ENS is a two-step process: First, ask the registry what resolver is responsible for the name, and second, ask that resolver for the answer to your query. The domain is owned by the owner till the deadline 
after that the owner has to renew it within 90 days' grace time. After the grace period, the name is released for registration by anyone with a temporary premium which decreases over a 28 days period to prevent domain squatters.
The released and registered names can be viewed in [Dune analytics dashboard](https://dune.com/makoto/ens-released-to-be-released-names). Anyone can extend a domain’s expiration period but the ownership is still maintained by the owner 
of that domain. Currently registration and renewal cost $5/year for names that are five characters or longer. Four character names cost $160/year, and three character names cost $640/year. Domains are bought using Eth similarly gas fees are paid in Eth.

### ENS Domains as NFTs 

ENS domains with .eth are NFTs because they are in ERC-721 standards. All NFTs have a unique uint256 tokenID from which we can convert to the actual content or art or data. The domains with .eth are traded and exchanged like NFTs. The tokenID’s are globally unique.

**Deriving tokenID from the ENS name**
For example, to derive tokenID for the domain harry.eth we use the following code to implement.

```
const ethers = require('ethers')
const BigNumber = ethers.BigNumber
const utils = ethers.utils
const name = 'harry'
const labelHash = utils.keccak256(utils.toUtf8Bytes(name))
const tokenId = BigNumber.from(labelHash).toString()
```
we are using etherjs predefined functions to produce the keccak256 hash of the name, and we are converting the hash to the number using BigNumber method, then it is converted to a string.


    


---
## Evaluation





##### Which of the following is correct about renewal of ENS domains?  

- [ ]  Renewal must be done within 1 day after deadline
- [x]  Anyone can extend expiration period of any domain but the ownership of the domain is retained by the owner
- [x]  The grace period for renewal is 90 days
- [ ]  Only owner can renew or extend the domain





##### What are the following the user must do after purchasing the domains?  

- [x]  User must set the resolver address. It can be either public resolver or custom resolver.
- [x]  User must set the wallet addresses and text records like emails if required
- [ ]  Users must pay different amount for different features after purchasing the domains
- [x]  Users are required to setup the reverse records for the replacing of addresses with domain names such that names are displayed instead of addresses





##### Which of the following are correct about ENS domains as NFTs?  

- [ ]  Every ENS domains are NFTs
- [ ]  ENS domains are not NFTs
- [x]  ENS domains with .eth tld is an NFT but others are not
- [x]  Vitalik.eth can be an NFT but harry.xyz cannot be an NFT

    


---
## Improvement proposals

**ENS Working - EIP-137**

The EIP-137 proposal explains the working model of the ENS protocol, including the registry and resolver contracts. It describes the functions and requirements of these contracts, as well as the
option for adding subdomains. Finally, it outlines the main improvements to the ENS protocol including the public resolver contract.

**Reverse solution-EIP-181**

The purpose of this proposal is to reverse the process for ENS domains. For example, if we look at Etherscan, we can see that the "from" ID is currently an address. However, after this proposal reverse 
solution is enacted, the address will be replaced with the ENS domain name only if that address owns a ENS domain and has set a primary ENS name. Anyone can configure a name to resolve to an address, 
regardless of ownership of that address. Reverse records allow the owner of an address to claim a name as authoritative for that address.

**Text records-EIP-634**

This proposal implements a new interfaceID for storing the text records by which ENS domain can be used instead of the records. We can link global keys like email, discription, url etc. We can link 
public keys like social media handles, github handles, etc. This is the main motive of this proposal.


    


---
## Your Info





| Label | Type | Required |
| ----------- | ----------- | ---- |
| Nick Name        | PublicShortInput   |  true    |


    


---
## Footer
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

## Best ENS VIDEOS 

### ENS Sessions
- Session 1: DNS Integration - https://www.youtube.com/watch?v=wSF_f3cJpy8
- Session2: Governance - https://www.youtube.com/watch?v=sGej7AbD_EY
- Session3: Layer 2 - https://www.youtube.com/watch?v=9DdL7AQgXTM
- Session4: Show & Tell - https://www.youtube.com/watch?v=tZWRO6srhZw

### ETHGlobal
- Session: https://www.youtube.com/watch?v=26JAdqjcrDI 

### ENS Workshops
- ENS Workshop 1: ENS as NFT v2 (aka Name Wrapper) - https://www.youtube.com/watch?v=MRiBdqE3pDc
- ENS Workshop 2: ENS name as web3 profile - https://www.youtube.com/watch?v=Eiq1m2iNK6I


### References
https://discuss.ens.domains/t/second-draft-of-the-ens-dao-by-laws-for-comment/11462

### Working Groups
https://discuss.ens.domains/t/ep12-social-working-group-rules/12953

https://discuss.ens.domains/t/ep14-social-dissolve-community-working-group/12982

https://discuss.ens.domains/t/ens-dao-town-hall/12751/17

https://www.figma.com/file/Acprf74LL8mfRAehfyQZir/ENS---Podarchy-(alisha.eth)?node-id=0%3A1

### Steward
https://discuss.ens.domains/t/how-it-will-work-steward-nominations/9212

https://discuss.ens.domains/t/steward-election-q3-q4-2022/13185

### ENS Dashboard
https://datastudio.google.com/u/0/reporting/8785928a-71d5-4b17-9fea-fe1c937b064f/page/RoKgC

ENS Constitution
https://discuss.ens.domains/t/proposed-ens-constitution/814
https://ensdao.eth.limo/constitution.pdf  (First Four Pages)
https://docs.ens.domains/v/governance/ens-dao-constitution

Proposal Process
https://docs.ens.domains/v/governance/process#the-rfp-process


### Community Mods
https://twitter.com/serenae_fansubs
https://twitter.com/realZadok7

### ENS Grants
Airtable form to notify ENS that you have submitted your grant: 

https://airtable.com/shrtIhtC5VZJzJnvU

(and to make sure the tag gets added)

Some context on grant ideas
The Grant should be focused on accomplishing the following for ENS:
Usability - improving the user experience
Community - growing the ecosystem
Tooling - improving the developer experience
Governance - building tools and enhancements for governance
Education - content creation and initiatives to improve educational resources

https://docs.google.com/document/d/1b7ulHiSz6db9YN5ESg2hPacTJUcqGZGvkMh5AeBMyVc/edit

I would browse through current projects on Gitcoin too: 
https://gitcoin.co/grants/explorer/?page=1&limit=12&me=false&sort_option=weighted_shuffle&collection_id=false&network=mainnet&state=active&profile=false&round_num=0&customer_name=false&sub_round_slug=false&collections_page=1&grant_regions=&grant_types=&grant_tags=*ENS&tenants=&idle=true&featured=true&round_type=false&tab=grants

(sorry that was a long link)



What does it do?
What have you done?
What are you doing?
https://airtable.com/shrtIhtC5VZJzJnvU

https://hackmd.io/zxAcn501TlKUHcEwQXYi3Q


https://docs.google.com/document/d/1b7ulHiSz6db9YN5ESg2hPacTJUcqGZGvkMh5AeBMyVc/edit
    
