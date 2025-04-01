---
timezone: UTC+8
---


# Ye

1. 自我介绍
    清华-南加大 Communication Data Science 25'硕士在读，链上数据分析2年经验，Dune [@wyeeeh](https://dune.com/wyeeeh)，X [@wyeeeeh](https://x.com/wyeeeh)，Optimism NumbaNERDs 分析师，入选Optimism RetroPGF Round 3 & Round 6 头部贡献者。

2. 你认为你会完成本次残酷学习吗？
   有激励就有野心，之前完成过Sixdegree Lab和BuidlerDAO发起的Dune Analytics共学计划，DeFiHackLabs发起的[Solidity残酷共学计划](https://basescan.org/token/0xb05d424943350adfadec4731cd54f12cc45e8c5c?a=0x7935D3A4beC9Dfe119bA2f7a1e977C406687Ac9C)，以及LXDAO发起的[第一期Optimism残酷共学计划](https://github.com/wyeeeh/Optimism)，有了这些积累，我认为我会完成这次学习。

3. 你的联系方式
   Telegram: [@wyeeeh](https://t.me/wyeeeh)


## Notes

<!-- Content_START -->

### 2025.03.31
**阅读文章：[Blockspace Charters: Superchain-first Governance](https://gov.optimism.io/t/season-6-introducing-blockspace-charters-superchain-first-governance/8133)**

#### 关键概念
1. [Law of Chains](https://github.com/ethereum-optimism/OPerating-manual/blob/main/Law%20of%20Chains.md)
   - 类似于Optimism Collective的[Operating Manual](https://github.com/ethereum-optimism/OPerating-manual/blob/main/manual.md)。
   - 它定义了集体治理的指导原则，为不同类型的超级链区块空间提供具体的实施细节。
   - 但没有定义投票周期、法定人数等具体机制。
2. Superchain Registry 注册表
   - 在 Blockspace 宪章框架中发挥关键作用，作为超级链组成部分的可访问索引。
   - 充当根据特定宪章接受哪些链的真相来源，并记录为每条链选择的特定配置值。用于存储和管理链的注册信息。
   - 纳入超级链注册表仅意味着纳入超级链。 超级链注册表实施了一个可扩展的分类系统，以清楚地划分哪些链属于哪些标准（因此属于哪个区块空间章程）
3. Incremental Rollout (Beta Registry) 增量测试版注册表
   -  (这部分没太看懂，明天继续研究)允许将一些初始链加入第一阶段安全理事会和超级链注册表

### 2025.04.01
**重读OP Stack及OP Superchain文档**
#### OP Stack
**文章：[Getting started with the OP Stack](https://docs.optimism.io/stack/getting-started)**
- 定义：OP Stack 是一个标准化、共享和开源的开发堆栈，为 Optimism 提供支持，由 Optimism Collective 维护。OP Stack 是支持 Optimism 的所有软件。随着 Optimism 的发展，OP Stack 也将不断发展。
- OP Stack 可以被视为软件组件，它既可以帮助定义 Optimism 生态系统的特定层，也可以在现有层中充当模块的角色。 尽管 OP Stack 目前的核心是运行 L2 区块链的基础设施，但 OP Stack 理论上可以扩展到底层区块链之上的层，包括区块浏览器、消息传递机制、治理系统等工具。
- 可以理解OP Stack是包含所有OP相关的开发组件，而Superchain是其中一部分。

#### Superchain
**文章：[Superchain Explainer](https://docs.optimism.io/superchain/superchain-explainer)**
- 继 Bedrock 之后，OP Stack 的下一个重大可扩展性改进是引入**超级链(Superchain)的概念**：共享Bridge、DAO、Upgrade、通信层等的链网络，所有这些都构建在 OP Stack 上。Superchain可以实现将把 OP 主网和其他链合并到一个统一的 OP 链网络（即超级链内的链）中。
- 超级链是一个 L2 链网络，称为 OP 链，共享安全性、通信层和开源技术堆栈。然而，与多链设计不同，这些链是标准化的，旨在用作可互换的资源。这使得开发人员能够构建以整个超级链为目标的应用程序，并抽象出应用程序运行的底层链。
- Bedrock引入了SystemConfig合约，开始直接用L1智能合约定义一些L2链。这可以扩展为将定义 L2 的所有信息放在 L1 上。包括生成唯一的链ID、区块gas limit等关键配置值等。
- (4.1 备注：未完待续)


<!-- Content_END -->
