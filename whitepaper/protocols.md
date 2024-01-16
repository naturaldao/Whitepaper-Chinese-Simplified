---
description: 各种治理协议的交联是非常复杂的。
---

# PoV（价值证明）中的治理协议

如前所述，道易程PoV中有七大治理协议：

* 智能公器硬核协议（Smart Commons' Hardcore Protocol）
* 去中心化铸造协议 Decentralized Minting Protocol
* 去中心化自治基金协议（Protocol of Decentralized Autonomous Fund）
* 估值通证供应协议（Protocol of Valuation Token's Supply）
* 计量单位通证协议（Protocol of Unit Token）
* 去中心化交易协议（Protocol of Decentralized Exchange）
* 通用支付协议（Protocol of Universal Payment）

## **智能公器硬核协议（Smart Commons' Hardcore Protocol）** <a href="#daohardcore" id="daohardcore"></a>

* 智能公器硬核协议涵括智能公器所需要的基础资料如插槽ID、项目英文名称、项目Logo（SVG格式，建议不超过6K，否则实在太贵）、项目描述（可以是宣传口号Slogan）、创建时间（平台记录）、创始成员（匿名，只是ETH地址），专属估值通证的名称、简称和符号等等。
* 在设置智能公器时，创建者可以手工添加一些地址到该智能公器作为其初始成员。地址上限为64人。
* 该协议还包含智能公器的升级规则：它的dApp必须是可靠的。这意味着它的dApp一旦部署就不能被任何人修改。\
  如果你知道使命是[智能合约的可组合性](https://ethereum.org/zh/developers/docs/smart-contracts/composability)，你就知道这条规则有多重要。从技术上讲，代理模式（Proxy Pattern）对于几乎所有智能公器来说都是一种自杀方式。如果您发现dApp中存在错误，请修复它并将其作为新的dApp部署到以太坊，然后返回道易程将其逐出为智能公器的新版本。\
  因此，数据分离（Data Separation）可能是一些dApp开发的最佳策略，并且合约迁移（Contract Migration）也可能可行。\
  如果您需要一些帮助来了解dApp升级，[推荐阅读本文](https://dev.to/joshuajee/smart-contract-upgrade-1ec2)。

## **去中心化铸造协议 Decentralized Minting Protocol** <a href="#deauthentication" id="deauthentication"></a>

铸造（Minting）即是合约交互，它是智能合约间最基础的行为。DAism摒弃了当前虚幻的DID概念，为smart common的创建采用了极简且极为可靠的去中心化认证手段，即smart common的创建始于某个合约地址下的智能合约的Minting请求而与当前其它任何DID无关。Mint协议可以证明一个smart common源于哪个智能合约，而此智能合约即能让所有人知道其功用或目的，机制非常简单也绝对真实可靠。它是创建smart common的唯一方式，也可作为smart common的创世证据，解决智能体及其专属的估值通证和dApp基于哪个核心智能合约的这一真实信息的关联问题。

同时，该协议中还包含了一个智能公器子协议，其名称为 SC0（意为Smart Commons 0）。即Minting操作，也就是宣布某个智能合约或某个dApp（某些智能合约的组合）自身成为以太坊的公共资源（Public Goods）——我们称其为智能公器（Smart Commons ）。这也就是说，接受道易程治理的dApp，即为智能公器。

> **SC0 v0.1**
>
> 用一个dApp Mint一个Smart Commons意味着它接受了本协议的排他治理。
>
> 我们都知晓dApp的所有者（或开发者或管理者）全部匿名这一事实。因为匿名，没有谁可证明其为任何权利的享有者，也没有谁可证明谁是任何责任的背负者。
>
> 1、接受道易程的治理。
>
> 2、无著作权
>
> 匿名意味着其开发的dApp完全贡献至公共领域，将其归属于智能公器（Smart Commons），除能够享受价值证明（Proof-of-Value）带来的奖励外，彻底放弃（割裂）所有其它权利，包括所有相关权利和邻接权利。
>
> 3、无责任
>
> 匿名意味着这个世界上，没有（无法确定）谁对一个dApp及其专属估值通证提供任何形式的担保，没有谁（无法确定）承担任何连带责任。
>
> 当使用或调用本dApp，或投资本智能公物专属估值通证时，任何人不得暗示本智能公器或其关联的任何人（所有者、开发者、管理者）为他或她的行为背书。

## **去中心化自治基金协议（Protocol of Decentralized Autonomous Fund）** <a href="#daf" id="daf"></a>

道易程的价值证明给每个smart common都提供了可以永续的奖励。每家smart common也都有一个极简的去中心化自治基金（Decentralized Autonomous Fund），该 DAF 可以调整奖金的分配，包括分配给哪些账户、每个账户被分配的额度（百分数）。

## **估值通证供应协议（Protocol of** Valuation **Token's Supply）** <a href="#tokensupply" id="tokensupply"></a>

任何一个智能公器都会发行其专属的估值通证（中文也可以称其为估值代币）。估值通证的主要作用是让投资者参与dApp的价值评估，并为道易程的共识价值证明提供奖金来源。

该协议主要定义估值通证的技术标准、名称、缩略符、Logo及其发行量、发行价。

估值通证协议和IADD有非常密切的关系，可以说它也是构成 IADD 网络的重要协议之一。

* 通证标准为EIP-3712。
* 估值通证全部发行到 IADD 网络，项目方1个都没有。它彻底革新了区块链长期不合理的代币市场供应机制，也是防范项目方和资本方联合操控市场甚至空手套白狼忽悠市场的重要手段！
* 发行标准都一致：发行总量为10,000,000,000个，发行价为 0.000000000000000000 vita。

## **计量单位通证协议（Protocol of Unit Token）** <a href="#utoken" id="utoken"></a>

计量单位通证是道易程的 IADD （去中心化交易和去中心化支付2合1网络）中，通过恒定乘积算法（constant product formula），为一切估值通证定价的通证。

这是道易程的一个核心创新。该协议的核心是一种叫uToken（Unit Token的简称）的单位通证。

1. uToken 由 ETH 锻造获取，亦即定价通证有一个非常独特的发行机制——你也可以理解为uToken是ETH的变体，其价值源于以太坊。uToken也是后面要介绍的 IADD 网络核心要素。uToken也是IADD网络的每一个交易对里面的必需通证。
2. uToken 是一种非常独特的通证。它是道易程定义的一种价格原器（单位通证），被定义为 1 uToken = 1 vita。和我们熟知的**国际单位制**的质量的基本单位类似，道易程有一套价格单位用于计算估值通证的价格。其中vita是**通证价格的基本单位**。
3. 道易程平台里面的一切估值通证的即时价格，都以价格原器 uToken 为基准，以 vita为计价单位，通过恒定乘积算法（constant product formula）计算获取。
4. vita是通证价格的基本单位。\
   计量通证 uToken 是道易程的去中心化交易和支付网络（IADD网络）中的价格原器（定价基准物），它的价格的基本单位为vita。那么也就是说，凡涉及到通证交易或者支付时，一律以 vita为价格的基本单位来标价。就支付来说，通证经济生态里的一切产品和服务的售价，也都以 vita为价格的基本单位来标价。如：\
   1 ISM = 0.01 vita\
   产品售价：0.5 vita/ kg\
   服务费：200 vita/ 小时

计量单位通证 uToken是道易程独创的价格单位制里的价格原器（定价基准物）。它会最大程度地降低估值通证应用的复杂度，也完全符合去中心化市场以及去中心化通用支付（结算）的需要。

### 为什么我们需要ETH的变体？

* ETH 错过了作为价格原型的机会，因为它的价值已经被美国的法定货币绑架了。 每当市场熊市的时候，一些矿工就因为ETH价格大幅下跌而不得不退出，充分说明了这一问题。
* &#x20;ETH采用的发行策略不利于快速扩张的市场，因此时它需要在短时间内大幅增加ETH的供应量。
* ETH是以太坊区块链的原生加密货币，与智能合约发行的通证不同。 这意味着它不遵守 ERC-20 或任何其他通证标准，使得它通常必须在供 dApp 使用之前要先铸造成 WETH（ERC-20 代币）。为了解决这个问题，创建变体的最佳策略是通过锻造。
* 在DAism的通证经济学中，作为价格原型，uToken的价格是恒定的。 这使其成为投资结算或日常支付的理想代币，类似于法定货币的日常使用。&#x20;
* 与其他一些代币不同，uToken 不能任意发行； 它需要有确定的价值来源。 此外，其发行必须遵循去中心化的方式以保持其信用。



## 去中心化交易协议（Protocol of Decentralized Exchange <a href="#dex-pay" id="dex-pay"></a>

* 该协议治理的是估值通证的交易机制。
* 仍然采用Bancor创新的自动化做市商（Automated Market Maker, AMM）。价格发现机制与 Bancor Network 或 Uniswap 类似。即IADD网络是道易程通用的去中心化交易和去中心化支付网络。 道易程以定价通证uToken、DAO专属的估值通证、恒定乘积方程式、智能合约构成IADD网络。
* 通过估值通证供应协议的协同，智能合约用算法独立治理流动性池，无需人参与。
* 估值通证在 IADD 网络有交易时，交易手续费（0.2%）作为奖金奖励给其所属DAO。

## 通用支付协议（Protocol of Universal Payment）

* 与去中心化自治基金会协议、计量单位通证协议、去中心化交易协议密切配合。
* 一切产品与服务的价格均以 vita 为价格单位。
* 购买产品或服务时，通过 IADD Network 完成不同币种的自动兑换。此时，uToken就是商家的结算通证。

## **其它与治理相关的技术探讨** <a href="#honor" id="honor"></a>

### **图片存储标准**

我们原创的图片存储标准意义重大：

* 首先应用于荣誉通证的链上存储。我们成功制订了EIP-2569（Saving and Displaying Image Onchain for Universal Tokens），以太坊已经收录（查询：[https://eips.ethereum.org/all](https://eips.ethereum.org/all)）。这意味着我们创立了面向整个以太坊应用的技术标准。
* 扩大应用到一切图片的存储。譬如我们已经将它应用到了去中心化媒体。

### **荣誉通证（Token of Honor）** <a href="#honor" id="honor"></a>

荣誉的记录和表彰，可以作为DAO发展的重要激励手段。

荣誉通证的应用面是非常广泛的，包含：

* 区块链领域的荣誉勋章（Medal of Honor）、纪念币（Commemorative Token）、纪念章、徽章、证书等等
* 具有收藏价值的游戏道具等——我们的荣誉通证是百分之百保存在链上的（包括图片）。

这是我们开发的简单的荣誉通证交易所的DEMO：

[https://1155.goh.cool/](https://1155.goh.cool/)

[https://honor.goh.cool](https://honor.goh.cool/latest)

### **UI标准与协议 UI Standard & Protocol**

为便于第三方开发道易程应用层的模块，我们未来还要提供UI标准。当然第三方贡献也行。

目前已确定使用的第三方协议有 Monkey King Protocol、ActivityPub。
