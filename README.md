# Awesome AI Resources

A curated list of AI learning and research-engineering resources, maintained by CUMT Alethic Insight Lab.

由 CUMT Alethic Insight Lab 维护的 AI 学习与研究工程资源清单。

---

## About | 关于本清单

This list curates stable, well-known, high-quality resources for AI study and engineering practice: papers, courses, official documentation, and major open-source projects. It is intended as a starting map for lab members and new contributors, not an exhaustive index.

本清单只收录稳定、知名、高质量的资源：论文、课程、官方文档与主流开源项目，为社团成员与新贡献者提供入门地图，而非求全的索引。

**Contribution | 贡献方式**: additions and corrections are welcome via Pull Request. Please only include stable links (arXiv, official GitHub, official documentation), with a one-line annotation in Simplified Chinese for each entry. This repository must not include private datasets, copyrighted materials without permission, leaked recruitment questions, or internal evaluation materials.

欢迎通过 Pull Request 补充或修正条目。每条资源请只使用稳定链接（arXiv、官方 GitHub、官方文档），并附一句简体中文注解。本仓库不得收录私有数据集、未经授权的版权材料、外泄的招新题目或内部评测材料。

---

## Contents | 目录

- [LLM Foundations | LLM 基础](#llm-foundations--llm-基础)
- [RAG & Retrieval | RAG 与检索](#rag--retrieval--rag-与检索)
- [Agents | Agent 智能体](#agents--agent-智能体)
- [Reinforcement Learning | 强化学习](#reinforcement-learning--强化学习)
- [Multimodal | 多模态](#multimodal--多模态)
- [Reasoning & Evaluation | 推理与评测](#reasoning--evaluation--推理与评测)
- [AI Infrastructure | AI Infra](#ai-infrastructure--ai-infra)
- [Engineering Practice | 工程实践](#engineering-practice--工程实践)

---

## LLM Foundations | LLM 基础

| Resource | 说明 |
| --- | --- |
| [Attention Is All You Need](https://arxiv.org/abs/1706.03762) | Transformer 开山之作，现代 LLM 的架构基础。 |
| [GPT-3: Language Models are Few-Shot Learners](https://arxiv.org/abs/2005.14165) | 展示规模效应与上下文学习能力的里程碑论文。 |
| [LLaMA: Open and Efficient Foundation Language Models](https://arxiv.org/abs/2302.13971) | 开源基座模型的代表性工作，影响后续大量模型。 |
| [Stanford CS336: Language Modeling from Scratch](https://stanford-cs336.github.io/) | 从零实现语言模型的斯坦福课程，工程含量极高。 |
| [Hugging Face NLP Course](https://huggingface.co/learn/nlp-course) | Transformers 生态官方免费课程，中文友好。 |
| [karpathy/nanoGPT](https://github.com/karpathy/nanoGPT) | 约千行代码训练 GPT，最适合动手读源码。 |
| [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) | 图文详解 Transformer 内部机制的经典博文。 |

## RAG & Retrieval | RAG 与检索

| Resource | 说明 |
| --- | --- |
| [RAG: Retrieval-Augmented Generation](https://arxiv.org/abs/2005.11401) | 检索增强生成原始论文，RAG 范式的起点。 |
| [Dense Passage Retrieval (DPR)](https://arxiv.org/abs/2004.04906) | 稠密向量检索的代表性方法，理解向量召回必读。 |
| [facebookresearch/faiss](https://github.com/facebookresearch/faiss) | Meta 官方向量相似度搜索库，工业级检索底座。 |
| [huggingface/sentence-transformers](https://github.com/huggingface/sentence-transformers) | 最流行的句向量编码库，Embedding 入门首选。 |
| [run-llama/llama_index](https://github.com/run-llama/llama_index) | 主流 RAG 框架，数据连接与索引抽象完善。 |
| [langchain-ai/langchain](https://github.com/langchain-ai/langchain) | LLM 应用编排框架，生态与集成最广。 |
| [vibrantlabsai/ragas](https://github.com/vibrantlabsai/ragas) | 面向 RAG 系统的自动化评测框架。 |

## Agents | Agent 智能体

| Resource | 说明 |
| --- | --- |
| [ReAct: Synergizing Reasoning and Acting](https://arxiv.org/abs/2210.03629) | 推理与行动交替的经典范式，Agent 基础论文。 |
| [Toolformer](https://arxiv.org/abs/2302.04761) | 让模型自学调用外部工具的早期代表作。 |
| [Voyager](https://arxiv.org/abs/2305.16291) | Minecraft 中的终身学习 Agent，长程规划经典案例。 |
| [microsoft/autogen](https://github.com/microsoft/autogen) | 微软多智能体协作框架，对话式 Agent 编排。 |
| [SWE-agent/SWE-agent](https://github.com/SWE-agent/SWE-agent) | 让 Agent 自动修复 GitHub issue 的学术研究项目。 |
| [OpenHands/OpenHands](https://github.com/OpenHands/OpenHands) | 开源软件开发 Agent 平台，代码执行闭环完整。 |
| [OpenAI Cookbook: Agents](https://cookbook.openai.com/) | OpenAI 官方 Cookbook，含函数调用与 Agent 实战示例。 |

## Reinforcement Learning | 强化学习

| Resource | 说明 |
| --- | --- |
| [Sutton & Barto: Reinforcement Learning (2nd ed.)](http://incompleteideas.net/book/the-book-2nd.html) | 强化学习标准教材，作者官方公开电子版。 |
| [OpenAI Spinning Up](https://spinningup.openai.com/) | OpenAI 官方 RL 入门教程，理论代码兼顾。 |
| [Playing Atari with Deep RL (DQN)](https://arxiv.org/abs/1312.5602) | 深度强化学习开山之作。 |
| [Proximal Policy Optimization (PPO)](https://arxiv.org/abs/1707.06347) | 最广泛使用的策略梯度算法，RLHF 核心组件。 |
| [InstructGPT: Training LMs to Follow Instructions](https://arxiv.org/abs/2203.02155) | RLHF 对齐的奠基性论文，理解后训练必读。 |
| [Farama-Foundation/Gymnasium](https://github.com/Farama-Foundation/Gymnasium) | RL 环境标准接口，OpenAI Gym 的社区继任者。 |
| [DLR-RM/stable-baselines3](https://github.com/DLR-RM/stable-baselines3) | PyTorch 版主流 RL 算法可靠实现，实验复现利器。 |

## Multimodal | 多模态

| Resource | 说明 |
| --- | --- |
| [An Image is Worth 16x16 Words (ViT)](https://arxiv.org/abs/2010.11929) | 视觉 Transformer 奠基论文，多模态编码器基础。 |
| [CLIP: Learning Transferable Visual Models](https://arxiv.org/abs/2103.00020) | 图文对齐经典模型，多模态表征学习必读。 |
| [BLIP: Bootstrapping Language-Image Pre-training](https://arxiv.org/abs/2201.12086) | 视觉语言预训练代表作，图文任务通用框架。 |
| [LLaVA](https://github.com/haotian-liu/LLaVA) | 开源视觉指令微调标杆项目，VLM 复现首选。 |
| [Segment Anything (SAM)](https://arxiv.org/abs/2304.02643) | 通用图像分割基础模型，提示式视觉范式。 |
| [huggingface/diffusers](https://github.com/huggingface/diffusers) | 扩散模型官方标准库，文生图实践入口。 |
| [QwenLM/Qwen3-VL](https://github.com/QwenLM/Qwen3-VL) | 通义千问多模态系列，中文生态最强的开源 VLM 之一。 |

## Reasoning & Evaluation | 推理与评测

| Resource | 说明 |
| --- | --- |
| [Chain-of-Thought Prompting](https://arxiv.org/abs/2201.11903) | 思维链提示原始论文，激发推理能力的起点。 |
| [MMLU: Measuring Massive Multitask Understanding](https://arxiv.org/abs/2009.03300) | 使用最广的 LLM 综合能力基准。 |
| [HELM: Holistic Evaluation of Language Models](https://arxiv.org/abs/2211.09110) | 斯坦福提出的系统化 LLM 评测框架。 |
| [GPQA](https://arxiv.org/abs/2311.12022) | 研究生级高难度问答基准，检验深度推理能力。 |
| [EleutherAI/lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) | 社区标准 LLM 评测工具，覆盖主流基准。 |
| [open-compass/opencompass](https://github.com/open-compass/opencompass) | 上海 AI Lab 评测平台，中文榜单支持完善。 |

## AI Infrastructure | AI Infra

| Resource | 说明 |
| --- | --- |
| [vllm-project/vllm](https://github.com/vllm-project/vllm) | 最流行的 LLM 推理服务引擎，PagedAttention 开创者。 |
| [sgl-project/sglang](https://github.com/sgl-project/sglang) | 高性能推理框架，结构化生成与缓存优化突出。 |
| [NVIDIA/TensorRT-LLM](https://github.com/NVIDIA/TensorRT-LLM) | NVIDIA 官方推理优化库，GPU 极致性能部署。 |
| [deepspeedai/DeepSpeed](https://github.com/deepspeedai/DeepSpeed) | 微软大规模训练框架，ZeRO 显存优化标配。 |
| [NVIDIA/Megatron-LM](https://github.com/NVIDIA/Megatron-LM) | 张量并行与流水线并行训练的参考实现。 |
| [ray-project/ray](https://github.com/ray-project/ray) | 分布式计算框架，RLHF 与数据流水线常用底座。 |
| [PyTorch Distributed Docs](https://pytorch.org/tutorials/beginner/dist_overview.html) | PyTorch 官方分布式训练教程与文档入口。 |

## Engineering Practice | 工程实践

| Resource | 说明 |
| --- | --- |
| [fast.ai: Practical Deep Learning](https://course.fast.ai/) | 自顶向下的实战深度学习课程，适合快速上手。 |
| [Full Stack Deep Learning](https://fullstackdeeplearning.com/) | 从模型到产品的全链路 ML 工程课程。 |
| [GokuMohandas/Made-With-ML](https://github.com/GokuMohandas/Made-With-ML) | MLOps 最佳实践教程，覆盖实验到部署全流程。 |
| [DataTalksClub/mlops-zoomcamp](https://github.com/DataTalksClub/mlops-zoomcamp) | 免费开源 MLOps 训练营，动手实验体系完整。 |
| [huggingface/transformers](https://github.com/huggingface/transformers) | 预训练模型事实标准库，必读的工业级代码。 |
| [OpenAI Cookbook](https://github.com/openai/openai-cookbook) | LLM 应用开发官方示例集，提示与集成范式齐全。 |
| [d2l-ai/d2l-zh](https://github.com/d2l-ai/d2l-zh) | 《动手学深度学习》中文开源教材，代码可运行。 |

---

## License | 许可

This list is released under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/). All linked resources belong to their respective owners.

本清单以 CC0 1.0 发布；所列资源版权归各自作者与机构所有。
