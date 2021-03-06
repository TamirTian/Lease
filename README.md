
## Lease Protocol

> Just a few thoughts, it's not final.

* [English](./README.md)
* [中文](./README-zh.md)
* [Support our of Gitcoin](https://gitcoin.co/grants/353/lease)

Lease Protocol is an open protocol that enables the peer-to-peer lease of assets on the Ethereum blockchain.

![Borrow.png](./images/borrow-assets.jpg)
![Return.png](./images/return-assets.jpg)

The lessor provides the liquidity of lease assets for the Protocol, and Protocol will generate a lease order and broadcast it to the Mesh Network of 0x, that's easy to sell on multiple DEXs.

The lessee can borrow interesting assets on the multiple DEXs.

When the lessee begins the lease:
1. The lessee deposits a certain amount of cash pledge and rents into the Protocol. Then Protocol will transfer them to the decentralized bank (Compound/MakerDAO) to earn interest.
2. Also, the Protocol mint the ERC721 Token of the lease contract, and the lessor can trade on Asset Market.  

When the lessee returns the assets, then Protocol executes the following actions:
1. Return cash pledge and remaining rent to the lessee.
2. Transfer the rent to the lessor.
3. The lessee gets the reward from earning interest.

### About roles in Protocol
#### Lessor
The lessor provides the assets for the lessee and earns rent.

#### Lessee
The lessee borrows the assets from the lessor and pays the rent to the lessor. 

#### DEFI/Bank
The Protocol can earn additional interest at the bank of Compound/MakerDAO.

#### Asset Market
The user can exchange the asset to another asset; for example, SpiderDEX/Opensea can sell the ERC721 of lease contract that helps the user to reduce risk.

### Ignorable Extra Ideas
1. Peer-To-Peer Lease => ERC721 Contract => Contract Loan => Insurance
2. Peer-To-Peer Lease => ERC721 Contract => Earn Real-Time-Rent

#### Loan
The lease contract consists of cash deposit and rents as security so that the third party can provide the service of loan because the rent can be calculated and get in the expected period

#### Insurance
The loan may default, and the lease contract isn't completed. However, the insurance can provide the currency immediately that waits for the lease contract to be finished or liquidated. 

#### Earn Rent 
They can earn fees from the lessor wants to get money of rent every second/minute/hour that provides service that waits for the finished of the lease contract.
