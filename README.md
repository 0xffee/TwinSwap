
¡£

#Twinswap: TwinChain  distributed financial defi proposal
v1.0 August 29 2021
##Project vision
Twinswap project is based on the concept of digital twins to establish a new generation of defi technology framework and financial model with security, zero handling fee, high transaction frequency, unlimited capacity expansion and transparent and open data.

##Problems and bottlenecks of current defi Technology Architecture
###Transaction congestion
The processing capacity of the Ethereum main chain of pow consensus is limited, including the limitation of block capacity and frequency.
###High handling charges
A large number of defi transactions lead to high service charge gas prices in the main network
###Contract vulnerability attacked
The smart contracts that defi relies on are becoming more and more responsible, making it difficult to find and audit internal code vulnerabilities. Once attacked, the amount of loss often reaches hundreds of millions of dollars. Such safety accidents are more and more frequently.

##Overview of Twinswap Solution
Digital twin, called digital twin in English, is also called digital mapping and digital image. Digital twin is a simulation process that makes full use of physical model, sensor update, operation history and other data, integrates multi-disciplinary, multi-physical quantity, multi-scale and multi probability, and completes the mapping in the virtual space, so as to reflect the whole life cycle process of the corresponding physical equipment. Digital twin is to create a digital version of "clone" on the basis of a device or system.

Before the public blockchain goes online, a testnet chain will be built. For example, the test chain of Ethereum's Kovan and georli, on the one hand, is to test the basic functions, performance and stability for the main chain, which is used as various technical tests for the main chain. After the main chain goes online, the test chain will continue to maintain technical foresight. New functions will be implemented and verified on the testnet chain first. After it is determined that the target requirements are basically met, it will be synchronized to the main chain code, so as to officially upgrade the main chain. Therefore, the testnet chain and the main chain are a twin relationship.


###Advantages and disadvantages of testnet chain
####Adopt POS or POA consensus mechanism, and the framework is convenient.
####The Transaction fee is low. Most testnet chains will faucet testnet coins to encourage user to test function.
####By constructing multiple test chains, the transaction frequency and data capacity can be rapidly expanded
####It can quickly upgrade and patch system vulnerabilities
####The testnet chain is basically synchronized with the code base of the main chain, and various verified smart contracts of the main chain can be seamlessly deployed to the test chain.
####The defect is that the test chain needs to test new functions with few nodules, resulting in instability and easy to find downtime.


###Twinswap solution
####The twin test chain is used as the twin chain of the main chain to deploy the defi transaction contract
####Recruit margin verification nodes on the main chain, deploy multi signature wallets, and set up margin Dao community by the verifier. Issue Delphi transaction tokens of erc20 protocol for transaction margin, community governance, etc
####Synchronously establish erc20 contract tokens on the twin test chain and defi trading pool contracts. The transaction fee is the test currency.
####Establish a bridge gateway between the main chain and the test chain
####The trader deposits the trading margin into the margin erc20 wallet in the main chain, and synchronizes to the defi trading tokens of the main chain and the twin test chain. All transactions are carried out on the test chain.
####When a trader needs to withdraw the trading margin, he first sells the defi token on the test chain, and then sells the token on the main chain wallet to exchange it for the main chain currency.
####The block data of the twin test chain will be backed up in a timely, full and incremental manner to the node space of swam, filecoin and arweave distributed storage. When the twin test chain is down and the data is not synchronized, the verification node will restore to the recognized block height and continue to run or upgrade the node software.
###Advantages of twinswap scheme
####Adopt the POS or POA consensus mechanism to expand the capacity of multiple twin chains, and the framework is convenient
####Low handling fee
####By constructing multiple twin test chains, the transaction frequency and data capacity can be rapidly expanded
####It can quickly upgrade and patch system vulnerabilities
####The test chain is basically synchronized with the code base of the main chain, and various excellent smart contracts verified by the main chain can be seamlessly deployed to the twin test chain. It can rapidly expand the popular defi financial transaction mode
####The operator of the verification node has increased the fee income of defi token exchange
####Give full play to the huge storage space of the distributed storage node, timely back up the block data of the twin test chain, ensure that the data is open, fair and tamperable, and facilitate the timely recovery to the normal operation state.
####The guarantee funds deployed on the main chain and twin test chain sign more wallet contracts, which isolates the guarantee fund and the defi trading pool contract, ensures the capital security and reduces the risk of guarantee fund theft caused by the vulnerability of the defi contract.
##Summary
Twinswap introduces the concept of digital twin technology into the blockchain industry, draws lessons from the successful operation and maintenance mode of the existing main chain and test chain, gives full play to the security advantages of multiple wallet contracts, increases the income of compliance operation of verification nodes, and stimulates the economic incentive power. It provides defi traders with unlimited capacity expansion of high-frequency trading.
