
# TwinSwap: 链孪生 分布式金融DeFi 方案书
v1.0 August 29 2021
## 项目定位和愿景

TwinSwap 项目依据数字孪生的理念，建立安全，零手续费，高交易频率，无限扩容，数据透明公开的新一代DeFi 技术构架和金融模式。

## 当前DeFi 技术构架的问题和瓶颈
### 交易拥堵
    PoW共识的以太坊主链处理能力有限，包括块容量的限制和出块频率限制
### 手续费高
    大量DeFi 交易导致主网手续费gas 价格高企
### 合约漏洞被攻击
　　DeFi倚重的智能合约愈来愈负责，导致内部代码漏洞不易于发现和审计。一旦被攻击，损失金额往往达到上亿美元。这类安全事故高发。
　　
## TwinSwap 功能概述
数字孪生，英文名叫Digital Twin（数字双胞胎），也被称为数字映射、数字镜像。数字孪生，是充分利用物理模型、传感器更新、运行历史等数据，集成多学科、多物理量、多尺度、多概率的仿真过程，在虚拟空间中完成映射，从而反映相对应的实体装备的全生命周期过程。数字孪生就是在一个设备或系统的基础上，创造一个数字版的“克隆体”。
区块链公链在上线前会建设测试链，例如，以太坊的Kovan ，Georli 的测试链，一方面是测试主链的基本功能，性能和稳定性，为主链的作为各类技术测试。主链上线后，测试链会继续保持技术前瞻性，新功能会先在测试链上实施和验证，确定基本满足指标要求后，再同步到主链代码中，从而正式升级主链。所以，测试链与主链是一种孪生关系。

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

### 测试链的优势和缺陷
#### 采用PoS 或者 PoA 共识机制，构架便捷。
#### 手续费 低廉，大多测试链会赠送测试币，编译用户测试需求
#### 通过构架多条测试链可以迅速扩展交易频率和数据容量
#### 可以迅速升级修补系统漏洞
#### 测试链与主链的代码库基本同步，主链的被验证过的各类智能合约可以无缝部署到测试链上。
####  缺陷是测试链需要测试新功能，结节少，导致不稳定，容易发现宕机情况。

### TwinSwap 解决方案
#### 将孪生测试链作为主链的孪生链部署DeFi 交易合约
#### 在主链上招募保证金验证节点，部署多签钱包，由验证人组建保证金DAO社区。 发行 ERC20 协议的DeFi 交易代币，用于交易保证金，社区治理等
#### 同步在孪生测试链上建立 ERC20 合约代币，和DeFi 交易池合约。以测试币为交易手续费。
#### 在主链和测试链建立兑换桥接网关
#### 交易员在主链向保证金ERC20 钱包存入交易保证金，同步到主链和孪生测试链的DeFi 交易代币, 所有交易在测试链上进行。
#### 交易员需要提取交易保证金时，先在测试链上卖出DeFi 代币，再在主链钱包上卖出代币兑换成主链币。
#### 孪生测试链的区块数据将被及时全量和增量备份到 Swam,Filecoin, ARweave 分布式存储的节点空间中。当孪生测试链发生宕机和数据不同步时，由验证节点来恢复到公认的区块高度，继续开始运行或者节点软件升级。

### TwinSwap 方案的优点
#### 采用PoS 或者 PoA 共识机制，扩容多条孪生链构架便捷
#### 手续费 低廉
#### 通过构架多条孪生测试链可以迅速扩展交易频率和数据容量
#### 可以迅速升级修补系统漏洞
#### 测试链与主链的代码库基本同步，主链的被验证过的各类优秀智能合约可以无缝部署到孪生测试链上。可以迅速扩张热门DeFi 金融交易模式
#### 验证节点运营方增加了DeFi 代币兑换手续费收入
#### 发挥分布式存储节点巨大存储空间，及时备份孪生测试链的区块数据，保证数据的公开公正，不可篡改，便于及时恢复到正常运行状态。
#### 分别部署在主链和孪生测试链上的保障金多签钱包合约，隔离了保障金和DeFi交易池合约，保障了资金安全，降低了DeFi合约漏洞导致保障金被盗的风险。


## 总结
TwinSwap 将数字孪生技术理念引入区块链行业，借鉴已有主链和测试链的成功运维模式，发挥多签钱包合约的安全优势，增加验证节点合规运营的收益，激发了经济激励动力。为DeFi 交易员提供了高频交易的无限扩容能力。

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
