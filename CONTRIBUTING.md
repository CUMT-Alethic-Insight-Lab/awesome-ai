# Contributing | 贡献指南

Thank you for helping improve this list. This document defines what we accept, how to write entries, and the pull request workflow.

感谢你愿意完善这份清单。本文档说明收录标准、条目写法与 PR 流程。

---

## Inclusion Criteria | 收录标准

| # | Rule | 规则 |
| --- | --- | --- |
| 1 | **Stable and well-known**: widely cited papers, established courses/textbooks, official documentation, major open-source projects with sustained maintenance. | **稳定知名**：高引论文、成熟课程与教材、官方文档、持续维护的主流开源项目。 |
| 2 | **Official sources only**: link to arXiv abstract pages, official GitHub repositories, or official project/documentation sites. No mirrors, re-uploads, blog reposts, or paywalled copies. | **只用官方源**：链接限 arXiv 摘要页、官方 GitHub 仓库、项目官网/官方文档；不收镜像、转载、搬运或付费墙副本。 |
| 3 | **High signal, not exhaustive**: 8–12 entries per category. Adding one entry usually means considering which existing entry it displaces. | **高信噪比而非求全**：每类 8–12 条；新增一条通常意味着考虑替换掉哪一条。 |
| 4 | **Relevant to the lab's scope**: AI study and research engineering — LLMs, RAG, agents, RL, multimodal, reasoning, evaluation, data, infra, serving, and engineering practice. | **契合社团方向**：AI 学习与研究工程——LLM、RAG、Agent、强化学习、多模态、推理、评测、数据工程、Infra、部署与工程实践。 |

## What We Do Not Accept | 不予收录

| Prohibited | 禁止内容 |
| --- | --- |
| Private or non-public datasets | 私有或非公开数据集 |
| Copyrighted material shared without authorization | 未经授权传播的版权材料 |
| Leaked recruitment/interview questions or internal evaluation material | 外泄的招新题目或内部评测材料 |
| Secrets of any kind: tokens, passwords, keys | 任何形式的密钥、口令、凭证 |
| QQ group numbers or QR codes | QQ 群号或二维码 |
| Real personal data (of applicants, members, or anyone else) | 真实个人信息（考生、成员或任何他人） |

## Entry Format | 条目写法

Entries live in Markdown tables, one row per resource:

条目放在 Markdown 表格中，每条一行：

```markdown
| [Name or Title](https://official-link) | 一句简体中文注解，客观说明它是什么、为什么值得读。 |
```

| Requirement | 要求 |
| --- | --- |
| Link text is the resource's official name or paper title (English as-is). | 链接文字用资源官方名称或论文原标题（英文保持原文）。 |
| The annotation is exactly one sentence of Simplified Chinese: objective, specific, no promotional adjectives. | 注解为一句简体中文：客观、具体，不使用宣传性形容词。 |
| Section headings follow `## English Name | 中文名`, with an `<a id="english-slug"></a>` anchor line above; add the new section to the Contents table too. | 分类标题遵循 `## 英文名 | 中文名`，上方加 `<a id="english-slug"></a>` 锚点行；新分类需同步加入目录表。 |
| UTF-8 encoding, no emoji anywhere. | 全文 UTF-8 编码，任何位置不使用 emoji。 |

## Workflow | PR 流程

1. Fork this repository and create a branch, e.g. `add/eval-benchmarks`.
   Fork 本仓库并新建分支，例如 `add/eval-benchmarks`。
2. Make your edits. One thematic change per PR (e.g. "add two serving entries") beats a mixed batch.
   完成修改。一个 PR 只做一类主题改动（如「新增两条部署条目」），避免混杂。
3. Verify every link you add resolves (GitHub repos exist, arXiv IDs match the intended paper, docs sites return 200).
   核验你新增的每个链接可达（GitHub 仓库存在、arXiv 编号与论文对应、文档站点返回 200）。
4. Commit with a Chinese Conventional Commit message, e.g. `docs: 新增推理分类两条近两年工作`。
   使用中文 Conventional Commits 信息提交，例如 `docs: 新增推理分类两条近两年工作`。
5. Open the PR. In the description, list the entries added/removed and confirm the link checks.
   发起 PR，在描述中列出增删条目并说明链接核验情况。

> 兜底：仓库配有每周一次的自动死链巡检（`.github/workflows/link-check.yml`，非阻断、不卡 PR）；巡检失败时维护者会收到通知并集中修复，贡献者无需为此操心。

6. A maintainer reviews against the criteria above; please respond to review comments promptly.
   维护者将按上述标准评审，请及时回复评审意见。
