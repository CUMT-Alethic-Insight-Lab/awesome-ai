# Awesome AI Resources

A curated list of AI learning and research-engineering resources, maintained by CUMT Alethic Insight Lab.

由 CUMT Alethic Insight Lab 维护的 AI 学习与研究工程资源清单。

---

## About | 关于本清单

This list curates stable, well-known, high-quality resources for AI study and engineering practice: papers, courses, textbooks, official documentation, and major open-source projects. It is intended as a reference map for lab members and new contributors, not an exhaustive index.

本清单只收录稳定、知名、高质量的资源：论文、课程、教材、官方文档与主流开源项目，为社团成员与新贡献者提供查阅地图，而非求全的索引。

**Contribution | 贡献方式**: additions and corrections are welcome via Pull Request. Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting. This repository must not include private datasets, copyrighted materials without permission, leaked recruitment questions, or internal evaluation materials.

欢迎通过 Pull Request 补充或修正条目，提交前请先阅读 [CONTRIBUTING.md](CONTRIBUTING.md)。本仓库不得收录私有数据集、未经授权的版权材料、外泄的招新题目或内部评测材料。

---

## How to Use This List | 怎么用这份清单

This list is a **reference map**, not a study plan. If you are new to the lab, start with the onboarding guide in [open-onboarding](https://github.com/CUMT-Alethic-Insight-Lab/open-onboarding): it provides the recommended learning order and hands-on path. Then use this list as an extended index — when the guide mentions a topic (e.g. RAG, agents, evaluation), jump to the matching section below via the Contents table for primary papers, textbooks, and tools.

这份清单是**查阅地图**，不是学习计划。新成员请先从 [open-onboarding](https://github.com/CUMT-Alethic-Insight-Lab/open-onboarding) 的导论树入手，按推荐顺序学习与练手；遇到导论中提到的方向（如 RAG、Agent、评测）时，再通过下方目录跳转到对应分类，延伸查阅原始论文、教材与工具。

---

## Contents | 目录

| Section | 分类 | 收录内容 |
| --- | --- | --- |
| [LLM Fundamentals](#llm-fundamentals) | LLM 基础 | 架构、基座模型、入门课程与教材 |
| [RAG & Retrieval](#rag-retrieval) | RAG 与检索 | 检索增强、向量检索、RAG 框架与评测 |
| [Agents](#agents) | Agent 智能体 | 智能体范式、协议、主流框架 |
| [Reinforcement Learning](#reinforcement-learning) | 强化学习 | RL 教材、经典算法、RLHF 与推理模型后训练 |
| [Multimodal](#multimodal) | 多模态 | 视觉语言模型、扩散模型、语音 |
| [Reasoning](#reasoning) | 推理 | 思维链、推理增强方法、推理模型复现 |
| [Evaluation & Benchmarks](#evaluation-benchmarks) | 评估与基准 | 主流基准、评测框架、竞技场榜单 |
| [Data Engineering](#data-engineering) | 数据工程 | 预训练语料、数据清洗与处理工具 |
| [AI Infrastructure](#ai-infrastructure) | AI Infra | 分布式训练、微调框架、算子优化 |
| [Serving & Deployment](#serving-deployment) | 部署与服务化 | 推理引擎、量化、本地部署 |
| [Engineering Practice](#engineering-practice) | 工程实践 | ML 工程、MLOps、应用开发实战 |

---

<a id="llm-fundamentals"></a>
## LLM Fundamentals | LLM 基础

| Resource | 说明 |
| --- | --- |
| [Attention Is All You Need](https://arxiv.org/abs/1706.03762) | Transformer 开山之作，现代 LLM 的架构基础。 |
| [GPT-3: Language Models are Few-Shot Learners](https://arxiv.org/abs/2005.14165) | 展示规模效应与上下文学习能力的里程碑论文。 |
| [LLaMA: Open and Efficient Foundation Language Models](https://arxiv.org/abs/2302.13971) | 开源基座模型的代表性工作，影响后续大量模型。 |
| [DeepSeek-V3 Technical Report](https://arxiv.org/abs/2412.19437) | 高性价比开源 MoE 基座技术报告，工程细节翔实。 |
| [Stanford CS336: Language Modeling from Scratch](https://stanford-cs336.github.io/) | 从零实现语言模型的斯坦福课程，工程含量极高。 |
| [Hugging Face NLP Course](https://huggingface.co/learn/nlp-course) | Transformers 生态官方免费课程，含中文版本。 |
| [karpathy/nanoGPT](https://github.com/karpathy/nanoGPT) | 约千行代码训练 GPT，最适合动手读源码。 |
| [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) | 图文详解 Transformer 内部机制的经典博文。 |
| [rasbt/LLMs-from-scratch](https://github.com/rasbt/LLMs-from-scratch) | 《Build a Large Language Model (From Scratch)》官方代码，逐章从零搭建并预训练 GPT。 |
| [《大语言模型》LLMBook-zh](https://github.com/LLMBook-zh/LLMBook-zh.github.io) | 赵鑫等编写的开源中文教材，系统覆盖预训练到应用全链路。 |

<a id="rag-retrieval"></a>
## RAG & Retrieval | RAG 与检索

| Resource | 说明 |
| --- | --- |
| [RAG: Retrieval-Augmented Generation](https://arxiv.org/abs/2005.11401) | 检索增强生成原始论文，RAG 范式的起点。 |
| [Dense Passage Retrieval (DPR)](https://arxiv.org/abs/2004.04906) | 稠密向量检索的代表性方法，理解向量召回必读。 |
| [Self-RAG](https://arxiv.org/abs/2310.11511) | 让模型自适应决定何时检索、如何反思检索结果。 |
| [BGE-M3](https://arxiv.org/abs/2402.03216) | 智源多语言多粒度 Embedding 模型，中文检索效果出色。 |
| [facebookresearch/faiss](https://github.com/facebookresearch/faiss) | Meta 官方向量相似度搜索库，工业级检索底座。 |
| [huggingface/sentence-transformers](https://github.com/huggingface/sentence-transformers) | 最流行的句向量编码库，Embedding 入门首选。 |
| [qdrant/qdrant](https://github.com/qdrant/qdrant) | Rust 编写的主流开源向量数据库，文档完善。 |
| [run-llama/llama_index](https://github.com/run-llama/llama_index) | 主流 RAG 框架，数据连接与索引抽象完善。 |
| [langchain-ai/langchain](https://github.com/langchain-ai/langchain) | LLM 应用编排框架，生态与集成最广。 |
| [microsoft/graphrag](https://github.com/microsoft/graphrag) | 微软基于知识图谱的 RAG 框架，适合全局性问答。 |
| [vibrantlabsai/ragas](https://github.com/vibrantlabsai/ragas) | 面向 RAG 系统的自动化评测框架。 |

<a id="agents"></a>
## Agents | Agent 智能体

| Resource | 说明 |
| --- | --- |
| [ReAct: Synergizing Reasoning and Acting](https://arxiv.org/abs/2210.03629) | 推理与行动交替的经典范式，Agent 基础论文。 |
| [Toolformer](https://arxiv.org/abs/2302.04761) | 让模型自学调用外部工具的早期代表作。 |
| [Voyager](https://arxiv.org/abs/2305.16291) | Minecraft 中的终身学习 Agent，长程规划经典案例。 |
| [A Survey on LLM-based Autonomous Agents](https://arxiv.org/abs/2308.11432) | 复旦团队的 LLM 智能体综述，构建记忆规划行动全图景。 |
| [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) | Anthropic 主导的工具与数据源开放协议，已成事实标准。 |
| [microsoft/autogen](https://github.com/microsoft/autogen) | 微软多智能体协作框架，对话式 Agent 编排。 |
| [huggingface/smolagents](https://github.com/huggingface/smolagents) | HF 轻量 Agent 库，代码即动作的简洁实现。 |
| [SWE-agent/SWE-agent](https://github.com/SWE-agent/SWE-agent) | 让 Agent 自动修复 GitHub issue 的学术研究项目。 |
| [OpenHands/OpenHands](https://github.com/OpenHands/OpenHands) | 开源软件开发 Agent 平台，代码执行闭环完整。 |
| [browser-use/browser-use](https://github.com/browser-use/browser-use) | 让 Agent 操作浏览器的热门开源项目。 |
| [OpenAI Cookbook: Agents](https://cookbook.openai.com/) | OpenAI 官方 Cookbook，含函数调用与 Agent 实战示例。 |

<a id="reinforcement-learning"></a>
## Reinforcement Learning | 强化学习

| Resource | 说明 |
| --- | --- |
| [Sutton & Barto: Reinforcement Learning (2nd ed.)](http://incompleteideas.net/book/the-book-2nd.html) | 强化学习标准教材，作者官方公开电子版。 |
| [《动手学强化学习》boyu-ai/Hands-on-RL](https://github.com/boyu-ai/Hands-on-RL) | 张伟楠等的中文开源教材仓库，配套代码可运行。 |
| [OpenAI Spinning Up](https://spinningup.openai.com/) | OpenAI 官方 RL 入门教程，理论代码兼顾。 |
| [Playing Atari with Deep RL (DQN)](https://arxiv.org/abs/1312.5602) | 深度强化学习开山之作。 |
| [Proximal Policy Optimization (PPO)](https://arxiv.org/abs/1707.06347) | 最广泛使用的策略梯度算法，RLHF 核心组件。 |
| [InstructGPT: Training LMs to Follow Instructions](https://arxiv.org/abs/2203.02155) | RLHF 对齐的奠基性论文，理解后训练必读。 |
| [Direct Preference Optimization (DPO)](https://arxiv.org/abs/2305.18290) | 免显式 RL 的偏好优化方法，实现简单应用广。 |
| [DeepSeek-R1](https://arxiv.org/abs/2501.12948) | 通过大规模强化学习激发推理能力，GRPO 算法出处。 |
| [Farama-Foundation/Gymnasium](https://github.com/Farama-Foundation/Gymnasium) | RL 环境标准接口，OpenAI Gym 的社区继任者。 |
| [DLR-RM/stable-baselines3](https://github.com/DLR-RM/stable-baselines3) | PyTorch 版主流 RL 算法可靠实现，实验复现利器。 |
| [huggingface/trl](https://github.com/huggingface/trl) | HF 官方 RLHF 工具库，覆盖 SFT/DPO/PPO/GRPO。 |

<a id="multimodal"></a>
## Multimodal | 多模态

| Resource | 说明 |
| --- | --- |
| [An Image is Worth 16x16 Words (ViT)](https://arxiv.org/abs/2010.11929) | 视觉 Transformer 奠基论文，多模态编码器基础。 |
| [CLIP: Learning Transferable Visual Models](https://arxiv.org/abs/2103.00020) | 图文对齐经典模型，多模态表征学习必读。 |
| [BLIP: Bootstrapping Language-Image Pre-training](https://arxiv.org/abs/2201.12086) | 视觉语言预训练代表作，图文任务通用框架。 |
| [Latent Diffusion Models](https://arxiv.org/abs/2112.10752) | Stable Diffusion 背后的核心论文，文生图技术基础。 |
| [Segment Anything (SAM)](https://arxiv.org/abs/2304.02643) | 通用图像分割基础模型，提示式视觉范式。 |
| [haotian-liu/LLaVA](https://github.com/haotian-liu/LLaVA) | 开源视觉指令微调标杆项目，VLM 复现首选。 |
| [huggingface/diffusers](https://github.com/huggingface/diffusers) | 扩散模型官方标准库，文生图实践入口。 |
| [openai/whisper](https://github.com/openai/whisper) | OpenAI 开源语音识别模型，多语种鲁棒性强。 |
| [deepseek-ai/Janus](https://github.com/deepseek-ai/Janus) | 统一理解与生成的多模态模型，Janus-Pro 影响广泛。 |
| [OpenGVLab/InternVL](https://github.com/OpenGVLab/InternVL) | 上海 AI Lab 开源 VLM 系列，榜单表现长期领先。 |
| [QwenLM/Qwen3-VL](https://github.com/QwenLM/Qwen3-VL) | 通义千问多模态系列，中文生态最强的开源 VLM 之一。 |

<a id="reasoning"></a>
## Reasoning | 推理

| Resource | 说明 |
| --- | --- |
| [Chain-of-Thought Prompting](https://arxiv.org/abs/2201.11903) | 思维链提示原始论文，激发推理能力的起点。 |
| [Self-Consistency Improves Chain of Thought](https://arxiv.org/abs/2203.11171) | 多路径采样投票，简单有效的推理增强。 |
| [STaR: Self-Taught Reasoner](https://arxiv.org/abs/2203.14465) | 让模型自学推理的早期自举方法。 |
| [Least-to-Most Prompting](https://arxiv.org/abs/2205.10625) | 由简到繁分解问题，提升复杂推理泛化。 |
| [Tree of Thoughts](https://arxiv.org/abs/2305.10601) | 将思维链扩展为可回溯的思维树搜索。 |
| [OpenAI o1 System Card](https://arxiv.org/abs/2412.16720) | o1 系列官方系统卡，推理时计算与评估细节的第一手资料。 |
| [huggingface/open-r1](https://github.com/huggingface/open-r1) | HF 对 DeepSeek-R1 的完全开源复现项目。 |
| [Towards Large Reasoning Models: A Survey](https://arxiv.org/abs/2501.09686) | 大型推理模型综述，梳理训练与推理时扩展方法。 |

<a id="evaluation-benchmarks"></a>
## Evaluation & Benchmarks | 评估与基准

| Resource | 说明 |
| --- | --- |
| [MMLU: Measuring Massive Multitask Understanding](https://arxiv.org/abs/2009.03300) | 使用最广的 LLM 综合能力基准。 |
| [HELM: Holistic Evaluation of Language Models](https://arxiv.org/abs/2211.09110) | 斯坦福提出的系统化 LLM 评测框架。 |
| [C-Eval](https://arxiv.org/abs/2305.08322) | 中文知识与推理综合评测基准，中文模型常用。 |
| [GPQA](https://arxiv.org/abs/2311.12022) | 研究生级高难度问答基准，检验深度推理能力。 |
| [MMMU](https://arxiv.org/abs/2311.16502) | 大学学科级多模态理解与推理基准。 |
| [SWE-bench](https://arxiv.org/abs/2310.06770) | 以真实 GitHub issue 修复衡量代码 Agent 能力。 |
| [LiveBench](https://arxiv.org/abs/2406.19314) | 持续更新的防污染动态基准。 |
| [Humanity's Last Exam](https://arxiv.org/abs/2501.14249) | 前沿学科专家级超高难度基准。 |
| [EleutherAI/lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) | 社区标准 LLM 评测工具，覆盖主流基准。 |
| [open-compass/opencompass](https://github.com/open-compass/opencompass) | 上海 AI Lab 评测平台，中文榜单支持完善。 |
| [LMArena (Chatbot Arena)](https://lmarena.ai/) | 基于人类偏好的众包对战榜单，业界公认风向标。 |

<a id="data-engineering"></a>
## Data Engineering | 数据工程

| Resource | 说明 |
| --- | --- |
| [The Pile](https://arxiv.org/abs/2101.00027) | EleutherAI 经典开源预训练语料，数据配比研究起点。 |
| [Dolma](https://arxiv.org/abs/2402.00838) | AI2 三万亿 token 开放语料，清洗流程完全公开。 |
| [FineWeb](https://arxiv.org/abs/2406.17557) | HF 发布的高质量网页语料，附完整过滤配方。 |
| [DCLM: DataComp for Language Models](https://arxiv.org/abs/2406.11794) | 数据筛选基准与最佳实践，数据策展方法论标杆。 |
| [huggingface/datasets](https://github.com/huggingface/datasets) | 数据集加载与处理的标准库，生态事实标准。 |
| [huggingface/datatrove](https://github.com/huggingface/datatrove) | HF 大规模语料处理流水线库，FineWeb 同款工具。 |
| [modelscope/data-juicer](https://github.com/modelscope/data-juicer) | 阿里开源的一站式 LLM 数据处理系统，中文文档完善。 |
| [togethercomputer/RedPajama-Data](https://github.com/togethercomputer/RedPajama-Data) | 复刻 LLaMA 配比的开放语料项目。 |
| [Common Crawl](https://commoncrawl.org/) | 最大规模公开网页存档，多数语料的上游来源。 |

<a id="ai-infrastructure"></a>
## AI Infrastructure | AI Infra

| Resource | 说明 |
| --- | --- |
| [Dao-AILab/flash-attention](https://github.com/Dao-AILab/flash-attention) | 精确注意力算子的显存与速度优化，训练推理标配。 |
| [NVIDIA/Megatron-LM](https://github.com/NVIDIA/Megatron-LM) | 张量并行与流水线并行训练的参考实现。 |
| [deepspeedai/DeepSpeed](https://github.com/deepspeedai/DeepSpeed) | 微软大规模训练框架，ZeRO 显存优化标配。 |
| [hpcaitech/ColossalAI](https://github.com/hpcaitech/ColossalAI) | 潞晨科技开源分布式训练框架，中文社区活跃。 |
| [huggingface/nanotron](https://github.com/huggingface/nanotron) | HF 轻量 3D 并行训练库，SmolLM 系列同款。 |
| [pytorch/torchtune](https://github.com/pytorch/torchtune) | PyTorch 原生微调库，与官方生态无缝衔接。 |
| [unslothai/unsloth](https://github.com/unslothai/unsloth) | 高效低显存微调工具，单卡微调开源模型首选。 |
| [NVIDIA/NeMo](https://github.com/NVIDIA/NeMo) | NVIDIA 全栈 LLM 训练与对齐框架。 |
| [ray-project/ray](https://github.com/ray-project/ray) | 分布式计算框架，RLHF 与数据流水线常用底座。 |
| [PyTorch Distributed Docs](https://pytorch.org/tutorials/beginner/dist_overview.html) | PyTorch 官方分布式训练教程与文档入口。 |

<a id="serving-deployment"></a>
## Serving & Deployment | 部署与服务化

| Resource | 说明 |
| --- | --- |
| [vllm-project/vllm](https://github.com/vllm-project/vllm) | 最流行的 LLM 推理服务引擎，PagedAttention 开创者。 |
| [sgl-project/sglang](https://github.com/sgl-project/sglang) | 高性能推理框架，结构化生成与缓存优化突出。 |
| [NVIDIA/TensorRT-LLM](https://github.com/NVIDIA/TensorRT-LLM) | NVIDIA 官方推理优化库，GPU 极致性能部署。 |
| [huggingface/text-generation-inference](https://github.com/huggingface/text-generation-inference) | HF 官方生产级推理服务，与 Hub 生态集成。 |
| [InternLM/lmdeploy](https://github.com/InternLM/lmdeploy) | 上海 AI Lab 推理部署工具箱，量化方案齐全。 |
| [ggerganov/llama.cpp](https://github.com/ggerganov/llama.cpp) | 纯 C/C++ 本地推理事实标准，GGUF 格式生态核心。 |
| [ollama/ollama](https://github.com/ollama/ollama) | 一键本地运行开源模型的主流工具，适合快速体验。 |
| [kvcache-ai/ktransformers](https://github.com/kvcache-ai/ktransformers) | 清华团队异构推理框架，单卡跑超大 MoE 模型。 |
| [AutoGPTQ/AutoGPTQ](https://github.com/AutoGPTQ/AutoGPTQ) | GPTQ 量化部署主流实现，INT4 推理常用。 |

<a id="engineering-practice"></a>
## Engineering Practice | 工程实践

| Resource | 说明 |
| --- | --- |
| [fast.ai: Practical Deep Learning](https://course.fast.ai/) | 自顶向下的实战深度学习课程，适合快速上手。 |
| [Full Stack Deep Learning](https://fullstackdeeplearning.com/) | 从模型到产品的全链路 ML 工程课程。 |
| [GokuMohandas/Made-With-ML](https://github.com/GokuMohandas/Made-With-ML) | MLOps 最佳实践教程，覆盖实验到部署全流程。 |
| [DataTalksClub/mlops-zoomcamp](https://github.com/DataTalksClub/mlops-zoomcamp) | 免费开源 MLOps 训练营，动手实验体系完整。 |
| [stas00/ml-engineering](https://github.com/stas00/ml-engineering) | 一线工程师的 ML 工程开源手册，训练调试经验密集。 |
| [huggingface/transformers](https://github.com/huggingface/transformers) | 预训练模型事实标准库，必读的工业级代码。 |
| [OpenAI Cookbook](https://github.com/openai/openai-cookbook) | LLM 应用开发官方示例集，提示与集成范式齐全。 |
| [d2l-ai/d2l-zh](https://github.com/d2l-ai/d2l-zh) | 《动手学深度学习》中文开源教材，代码可运行。 |
| [datawhalechina/llm-cookbook](https://github.com/datawhalechina/llm-cookbook) | DataWhale 中文 LLM 应用开发教程，入门友好。 |
| [dair-ai/Prompt-Engineering-Guide](https://github.com/dair-ai/Prompt-Engineering-Guide) | 提示工程系统指南，含中文翻译版本。 |
| [karpathy/nn-zero-to-hero](https://github.com/karpathy/nn-zero-to-hero) | Karpathy 从零手写神经网络的配套代码与讲义。 |

---

## License | 许可

This list is released under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/). All linked resources belong to their respective owners.

本清单以 CC0 1.0 发布；所列资源版权归各自作者与机构所有。
