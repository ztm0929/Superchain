---
timezone: UTC+8
---

> 请在上边的 timezone 添加你的当地时区(UTC)，这会有助于你的打卡状态的自动化更新，如果没有添加，默认为北京时间 UTC+8 时区


# 你的名字 stephanie

1. 自我介绍
上海大学通信工程专业，对区块链感兴趣。
2. 你认为你会完成本次残酷学习吗？
会
3. 你的联系方式（推荐 Telegram）
7259563054（telegram）
J-79756537（wx）

## Notes

<!-- Content_START -->

### 2025.03.31

1. What is a Blockspace Charter?

At a high level, a Blockspace Charter consists of three primary components: Criteria, Governing Policies, and Precommitments.

It provides a technical-focused governing document for the Superchain and defines the specific implementation details for different types of Superchain blockspace, similar to an "Operating Manual."

2. Why introduce a Blockspace Charter?

The Superchain is quickly blossoming into a robust ecosystem of OP Stack-based chains. However, these chains are not all technically equivalent:

Different chains may use different versions of the OP Stack—some projects have made modifications to the stack, and others are on outdated versions of it.

Even within chains that are on the same version, some may be configured differently — deployed with different values for various parameters, admin roles, and so on.

There is a need for:

Users and developers to easily understand what blockspace has which properties and guarantees.

Optimism Governance to understand how to make decisions about these different forms of blockspace, which may make different commitments and have different control structures.

The Law of Chains is a neutrality framework designed to provide a guiding light for the Superchain and its stakeholders to make decisions and uphold protections. However, the Law of Chains is intentionally agnostic to any specific details of the protocol, which means it can fail to provide clear guidance at the required granularity.

Blockspace Charters will act as the equivalent to the Operating Manual, providing the specific implementation details for different types of Superchain blockspace.

3. What does a Blockspace Charter include?

Criteria:

Version: The version of the OP Stack that the chain is using, as determined by commit-hash/release.

Configuration: The accepted range of parameterizations for the software in the OP Chain’s deployment, including both static (e.g., Chain ID) and dynamic variables (e.g., sequencer or upgrade keys).

Solvency: Ensuring that a chain’s history does not include any invalid withdrawals or invalid outputs that could cause the bridge to be undercollateralized.

Governing Policies:

Specific rules, procedures, and principles that stakeholders participating in the charter’s blockspace must follow.

Example: If a charter’s blockspace criteria require that upgrade keys be held by the Security Council, and allow the chain’s sequencer to be configured to be anybody, the governing policies could define:

The required behavior of the sequencer, which, if violated, would be grounds for removal.

The governance process (e.g., proposal type) by which governance could vote to remove the sequencer.

The signing procedure which would be subsequently taken by the Security Council to remove the offending sequencer.

The governing policies align with the Law of Chains principles to ensure protections for the charter’s blockspace.

Precommitments:

A commitment mechanism, outlining anticipated changes (or consistency) for future upgrades to the charter.

Precommitments help provide stakeholders with a clear understanding of the long-term vision and stability of the governance framework.

They can address critical aspects like fee split models, role separations, and technical parameters such as gas limits and fee margins.

4. How will Blockspace Charters be rolled out?

Superchain Registry:

The Superchain Registry will play a crucial role by serving as an accessible index of what chains are part of the Superchain.

It ensures that chains meet the criteria outlined in their respective Blockspace Charter before being added, ensuring consistency and security across the Superchain.

It is a public index that documents the configuration values of each chain and categorizes them under the appropriate charter.

Incremental Rollout (Beta Registry):

Some initial chains will be onboarded to the Phase 1 Security Council and Superchain Registry to test the process before the Standard Rollup Charter is ratified and scaled.

This phase is designed to help the Security Council become familiar with the end-to-end process and resolve any frictions before full implementation.

Improved Upgrade Proposal Process:

Upgrade proposals will correspond to specific Blockspace Charters.

Upgrade proposals must link to a pull request for an updated charter and provide justifications for any changes not covered in other sections.

The Impact Summary must demonstrate that all precommitments in the previous charter are preserved by the upgrade.

This ensures that the upgrade process is transparent, accountable, and stakeholder-focused, allowing the Collective to rigorously consider the impact on stakeholders.









### 2025.04.01

<!-- Content_END -->
