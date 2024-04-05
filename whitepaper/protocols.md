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
* 发行标准都一致：发行总量为1,000,000,000个，发行价为 0.000000000000000000 vita。

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
* &#x20;ETH采用的发行策略不利于快速扩张的市场，因此它需要在短时间内大幅增加ETH的供应量。
* ETH是以太坊区块链的原生加密货币，与智能合约发行的通证不同。 这意味着它不遵守 ERC-20 或任何其他通证标准，使得它通常必须在供 dApp 使用之前要先铸造成 WETH（ERC-20 代币）。为了解决这个问题，创建变体的最佳策略是通过锻造。
* 在DAism的通证经济学中，作为价格原型，uToken的价格是恒定的。 这使其成为投资结算或日常支付的理想代币，类似于法定货币的日常使用。&#x20;
* 与其他一些代币不同，uToken 不能任意发行； 它需要有确定的价值来源。 此外，其发行必须遵循去中心化的方式以保持其信用。

### 计量单位通证协议简介

该协议致力于价格单位制。这将是人类货币史上的一大创新！

在此协议中，基本价格单位为 vita，价格原器（定价基准物）为 uToken，也就是说一个 uToken的价格被定义为 1 vita。uToken的发行机制为ETH锻造，其精度为18位。这也意味着价格的最小单位 attovita 是 vita 的 10^-18。

### 计量单位制：

**名称：**计量单位通证（Unit Token，uToken）

**货币缩略符：**UTO

**标志：**

<figure><img src="../.gitbook/assets/vita-s.svg" alt="" width="64"><figcaption></figcaption></figure>

**基本单位：**vita

**辅币进位制：**1vita=100cent（分)

**单位：**

|          |          |          |          |
| -------- | -------- | -------- | -------- |
| **表示因数** | **中文词头** | **英文前缀** | **词头符号** |
| 10^24    | 尧\[它]    | yotta    | Y        |
| 10^21    | 泽\[它]    | zetta    | Z        |
| 10^18    | 艾\[可萨]   | exa      | E        |
| 10^15    | 拍\[它]    | peta     | P        |
| 10^12    | 太\[拉]    | tera     | T        |
| 10^9     | 吉\[咖]    | giga     | G        |
| 10^6     | 兆        | mega     | M        |
| 10^3     | 千        | kilo     | k        |
| 10^2     | 百        | hecto    | h        |
| 10^1     | 十        | deca     | da       |
| 10^-1    | 分        | deci     | d        |
| 10^-2    | 厘        | centi    | c        |
| 10^-3    | 毫        | milli    | m        |
| 10^-6    | 微        | micro    | μ        |
| 10^-8    | 聪        | sat      | s        |
| 10^-9    | 纳\[诺]    | nano     | n        |
| 10^-12   | 皮\[可]    | pico     | p        |
| 10^-15   | 飞\[母托]   | femto    | f        |
| 10^-18   | 阿\[托]    | atto     | a        |

### &#x20;计量单位通证协议的动机

要讨论计量单位通证的意义，就离不开与它关系密不可分的 IADD 网络。前面我们对 IADD 的缘起已经解释过。其中的重点为：

* 每个智能公器的估值通证都全部发行到 IADD 网络。和现在普遍采用的代币发售方式完全不同的是：项目方不负责估值通证发行、项目方也分配不到估值通证。杜绝项目方利用估值通证收割市场！
* 每个智能公器的估值通证都全部发行到了 IADD 网络， IADD 里的估值通证的价格能够反映市场的真实价值评判。

本协议的重点是价格单位制：

1. 国际单位制（法语：Système International d'Unités，简称SI）是世界上最普遍采用的标准度量系统。如1793年对重量（后改为质量）的定义为冰点下体积为一立方分米的纯水的重量。由此可见质量单位是通过一个参照物（标准物）定义出来的。而有了质量原器及其基本单位，万物的质量就都可以通过衡器中的算法计算出来。计量单位通证uToken是我们制定币价单位制的价格原器（定价基准物）。
2. IADD 网络采用了 Uniswap 的算法（恒定乘积方程式），但会以计量单位通证uToken代替ETH来计算估值通证的价格。
3. ETH锻造协议：通过锻造ETH而发行出计量单位通证，因此，uToken是ETH的变体——uToken不是凭空产生而是以ETH价值转移而发行。这是一种去中心化锻造模式，因为何时锻造以及锻造多少都是由用户自己决定。
4. 道易程锻造合约的启动，将意味着以太坊的同质化通证第一次有了自己独立自主的去中心化定价机制。也将意味着中心化世界的交易所对通证经济生态的巧取豪夺的时代将要终结。
5. 计量单位通证的另一个重要的应用领域是去中心化结算。因其它一切代币的价格都是波动的，无法被消费者持有而用于日常消费或者用于投资退出，只有uToken价格恒定（1 uToken ≡ 1 vita），因此它是道易程构建的通证经济生态里合格的通用支付币种（或称结算币种）。
6. 区块链支付的需求是随着区块链行业的发展越来越大的，而我们今天又无法计算出未来某个年月它的需求的大小，因此我们需要一种发行量理论上无限的通用支付币种。并且还需要能够伴随需求而进行双向调节的流动性池予以补充。

这是一个志在彻底摧毁中心化交易所对去中心化市场的干扰和破坏的方案！也是一个区块链结算的解决方案。

### 计量单位通证uToken的发行：ETH锻造 <a href="#forge" id="forge"></a>

本节内容需要你预先了解Uniswap的恒定乘积算法。具体请参阅以下资料。

Hayden Adams. 2018：[https://hackmd.io/@477aQ9OrQTCbVR3fq1Qzxg/HJ9jLsfTz?type=view.](https://hackmd.io/@477aQ9OrQTCbVR3fq1Qzxg/HJ9jLsfTz?type=view.)

以及vitalik Buterin发起的讨论：[Improving front running resistance of x\*y=k market makers](https://ethresear.ch/t/improving-front-running-resistance-of-x-y-k-market-makers/1281)

本协议将以ETH锻造模式，以ETH的美元价格的历史最高值为参考发行计量单位通证uToken。它的发行机制很独特：

1. 锻造初始化\
   协议启动（即合约启用）时，算法以每个计量单位通证所定义的价格即1 vita、ETH历史最高价（当前为4870美元）为基础进行初始化，即 1 ETH 可以锻造出4870个uToken。
2.  改良的恒定乘积（Imporved CPMM）算法提供锻造奖励\
    核心算法还是Uniswap的恒定乘积方程式。\
    x: 锻造池 ETH 数量\
    y: 锻造池 uToken 数量\
    $$x*y=k$$

    第N位早鸟的奖励为：\
    奖金\
    $$R = Δy_{n} = y_{n-1} - y_{n}= (k \div x_{0}) - (k \div x_{1}) = k \times(1/x_{0}-1/x_{1})$$

    其中\
    $$x_{n} = x_{n-1} + \Delta x_{n}$$

    最后一项就是第n个人锻造掉的ETH
3. 初始化K值\
   我们以至2022年11月30日 EIP-1559 已经burn掉的 ETH 为初始化的 ETH 总数。譬如我现在（20221130，00:00 香港时间）看到已经烧毁 2750240 个（https://etherchain.org/burn），其价值为：3320364758美元。这是全球用户的损失，因此我们假设这些ETH都进入了锻造池。\
   K = (2750240 \*3320364758)= 9,131,799,972,041,920 ≈ $9.1318e+15
4.  奖励公式即为：\


    $$x * y = 9.1318 * 10^{15}$$
5. 确定 ETH价格 再创新的最高价（假设为V2，之前的最高价假设为V1）的第二年，1个ETH 可锻造的uToken数量即调整至该最高价的数值（即V2），所有历史锻造者均会获得锻造补偿（即V2-V1）。\
   当锻造的ETH达到其总量的60%，兑换基数不再增加。或者但ETH价格达到487000美元时，兑换基数（487000）不再增加。这是一个和外部市场的价格熔断的机制。

## 去中心化交易协议（Protocol of Decentralized Exchange <a href="#dex-pay" id="dex-pay"></a>

* 该协议治理的是估值通证的交易机制。
* 仍然采用Bancor创新的自动化做市商（Automated Market Maker, AMM）。价格发现机制与 Bancor Network 或 Uniswap 类似。即IADD网络是道易程通用的去中心化交易和去中心化支付网络。 道易程以定价通证uToken、智能公器专属的估值通证、恒定乘积方程式、智能合约构成IADD网络。
* 通过估值通证供应协议的协同，智能合约用算法独立治理流动性池，无需人参与。
* 估值通证在 IADD 网络有交易时，交易手续费（0.2%）作为奖金奖励给其所属智能公器的开发者。

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

荣誉的记录和表彰，可以作为智能公器发展的重要激励手段。

荣誉通证的应用面是非常广泛的，包含：

* 区块链领域的荣誉勋章（Medal of Honor）、纪念币（Commemorative Token）、纪念章、徽章、证书等等
* 具有收藏价值的游戏道具等——我们的荣誉通证是百分之百保存在链上的（包括图片）。

这是我们开发的简单的荣誉通证交易所的DEMO：

[https://1155.goh.cool/](https://1155.goh.cool/)

[https://honor.goh.cool](https://honor.goh.cool/latest)

### **UI标准与协议 UI Standard & Protocol**

为便于第三方开发道易程应用层的模块，我们未来还要提供UI标准。当然第三方贡献也行。

目前已确定使用的第三方协议有 Monkey King Protocol、ActivityPub。
