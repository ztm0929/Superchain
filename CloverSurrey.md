---
timezone: UTC+8
---

> 请在上边的 timezone 添加你的当地时区(UTC)，这会有助于你的打卡状态的自动化更新，如果没有添加，默认为北京时间 UTC+8 时区


# 你的名字

1. 自我介绍
我是来自计科专业的Clover^^从朋友那里得知了这个项目，刚好也有很多朋友都报名了，觉得一起的话也许更容易坚持下去，所以报名了
虽然在区块链方面完全是小白，但是很期待接下来的学习！
3. 你认为你会完成本次残酷学习吗？
我希望我能完成本次残酷学习。每天半个小时到一个小时的学习时间应该不会太难完成。
4. 你的联系方式（推荐 Telegram）
邮箱：1922594228@qq.com
尝试注册telegram中……
24.04.01更新：已注册加入交流群

## Notes

<!-- Content_START -->

### 2025.03.31

基础知识复习：
区块记录了交易记录，区块连接成为了区块链

每个人拿到的交易记录顺序可能不同，因此需要↓

共识机制：决定了谁能记账并且得到所有人的认可
e.g:PoW工作量证明

区块链的形式使得给区块链中的记录造假变得非常困难（修改计算连接）


标准汇总章程笔记
何为Blockspace Charter：
以技术为重点的框架

创建Blockspace Charters的动机：
超级链基于op stack链，并且正在发展成一个强大的链生态系统。但是由于不同的链使用了不同版本的op stack，或是相同版本的链中的设置不同，导致了链生态系统的碎片化。因此需要一种简便的方式来理解哪些区块空间具有哪些属性和保障。

区块链法则（The Law of Chains）是一个中立框架，但是区块链法则故意对协议的具体细节保持中立。这使得它可以适用于协议的多个迭代版本，但也意味着它在上述细节层面可能无法提供明确的指导。
这使得区块链法则类似于Optimism集体（Optimism Collective）的工作宪法（Working Constitution）。它定义了集体治理的指导原则，却没有定义投票周期、法定人数等具体机制。
而区块空间章程（Blockspace Charters）则相当于操作手册，提供了不同类型的超级链（superchain）区块空间的具体实施细节。

实在看不懂。向AI求助得到：
通俗解释：

想象要建一座城市，这里有两个重要的文件：

《城市宪法》——（区块链法则）the law of chains
它规定了城市的基本原则，比如“居民安全第一”或“资源公平分配”。
这些是大的方向，不涉及具体怎么修路、怎么管理交通。
类似地，区块链法则为整个超级链生态系统设定了核心原则（如用户保护、去中心化），但不规定具体技术细节（比如用哪种算法或如何投票决策）。

《城市施工手册》——（区块空间章程）blockspace charters
这本手册会详细说明如何铺路、安装路灯、规划社区。
同样，区块空间章程是具体的技术指南，告诉开发者如何实现不同类型的区块空间（比如高性能链或高安全链），包括参数设置、权限分配等细节。

个人的混淆：
————————————
区块链法则 vs. 共识机制：

共识机制（如比特币的 PoW、以太坊的 PoS）是技术规则，解决“节点如何达成一致”的问题。

区块链法则是治理框架，解决“生态参与者如何共同决策和维护权益”的问题。两者不同，但共同支撑区块链运行。
————————————
两者的核心区别：

区块链法则					区块空间章程
像宪法，设定原则和方向			像操作手册，提供具体步骤
适用于所有协议版本，保持中立	针对特定需求定制技术细节
例：用户权益必须优先保护		例：如何设置链的 Gas 费用上限
简单来说，法则告诉你“为什么做”，章程告诉你“怎么做”。

由三个初级组件构成：
Criteria
Governing Policies
Precommitments

### 2025.04.01
前置基础知识学习更新：
区块链不等于比特币，比特币只是基于区块链技术的一种加密货币

2015 以太坊出现，逐渐成为主流的加密货币

比特币的密码学原理
-哈希/签名

cryptographic hash function
collision resistance 哈希碰撞
相同的输入映射到一个哈希值
没有什么高效的方法能人工创造哈希碰撞的情况
brute-force 暴力破解
因为哈希碰撞难以人工制造，故很难篡改内容却又不被检测出来（区块头的哈希值是由区块头+交易数据经过特定哈希运算得到的）
利用该特性，可以对数据的一致性进行检测
但这个特性是无法在理论上证明出来的
虽然一些哈希函数曾被认为是安全的，但随着技术的进步，发现了生成哈希碰撞的方法，这表明其安全性可能受到威胁。

哈希函数的单向性——无法反推原始输入，该特性也被成为hiding
确保了输入信息的安全性，避免泄露敏感数据。

puzzle friendly
这意味着计算哈希值的过程是不可预测的，无法通过输入直接得出哈希值。
*之所以叫puzzle friendly，是因为挖矿过程需要通过尝试大量随机数来找到符合要求的哈希值。这个过程没有捷径，只依赖于大量计算，因此被称为工作量证明

在比特币的系统中，开户的过程就是生成公私钥对。（基于非对称加密，比如rsa）
公钥类似账号，私钥类似密码
公私钥用来制作签名
————————————————————————————————————
Blockspace Charter由三个部分构成：
Criteria
Governing Policies
Precommitments
标准、管理政策和预先承诺。
标准：特定的技术参数，定义哪些链在给定章程的范围内。 
章程的标准应客观定义哪些链在其范围内。 通常，标准有两个组成部分：

1.版本（Version）：区块链所使用的OP Stack版本，由提交哈希（commit-hash）/版本发布决定。这指的是支持区块空间的特定协议代码。
2.配置（Configuration）：OP链部署中软件参数的接受范围。配置可以包括在创世时定义的静态变量，如链ID（Chain ID），以及动态变量，如链的排序器（sequencer）或升级密钥（upgrade keys）。配置的边界说明了这些选项必须落在的值范围内，才能满足宪章的标准。
3.偿付能力（Solvency）：确保链的历史记录不包括任何无效的提现或无效的输出，这些可能导致桥接（bridge）处于欠担保状态。

确保链的历史记录不包括任何无效的提现或无效的输出，这些可能导致桥接（bridge）处于欠担保状态


治理政策（Governing Policies） 是宪章区块空间中参与者所遵循的具体规则、程序和原则。
通常，治理政策将涉及不同配置角色应如何表现或互动，以及如何执行这些行为。
例如，如果某个宪章的区块空间标准要求升级密钥由安全委员会持有，并允许链的排序器配置为任何人，则治理政策可以定义：

1.排序器的必要行为，若违反该行为，将成为移除排序器的依据，并定义社区如何检查是否存在违反。
2.治理过程（例如提案类型），通过该过程，治理可以投票决定是否移除违反规定的排序器。
3.随后由安全委员会采取的签名程序，以移除违规的排序器。

-----关于sequencer
在区块链技术中，**Sequencer**（序列器）指的是一种特定类型的节点，主要用于处理和排序交易。Sequencer 在某些区块链架构（尤其是 Layer 2 解决方案，如 Rollups）中发挥重要作用。它的主要功能包括：

### 1. 交易排序
Sequencer 接收进入网络的交易请求，并将其按特定顺序排列。交易的顺序对状态的变化很重要，因此 Sequencer 确保交易以确定的方式被处理，以防止重放攻击和状态不一致性。

### 2. 提高性能
通过引入 Sequencer，Layer 2 解决方案可以在链下处理大量交易，然后将这些交易批量提交到主链。这种方法显著提高了交易吞吐量，降低了交易成本。

### 3. 管理状态更新
Sequencer 负责在交易被处理后管理区块链的状态更新。它确保所有交易按照正确的顺序执行，从而正确更新区块链的状态。

### 4. 可能的集中化问题
在某些实现中，Sequencer 可能引入集中化的问题，因为所有交易都必须通过一个或几个 Sequencer。这可能导致信任问题和潜在的单点故障。

### 5. 用于 Rollups
在 Rollup（例如 zk-Rollup 和 Optimistic Rollup）架构中，Sequencer 扮演着至关重要的角色，它负责收集用户交易并将它们打包以提交到主链，从而提高了整体网络的可扩展性。

总的来说，Sequencer 是区块链技术中用于提高交易处理效率和性能的重要组件之一。

### 2025.04.02
<!-- Content_END -->
