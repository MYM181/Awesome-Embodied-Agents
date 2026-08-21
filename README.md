# Awesome Embodied Agents


## Contents

- [1. Foundations and Generalist Policies](#1-foundations-and-generalist-policies)
- [2. Long-Horizon Planning and Embodied Reasoning](#2-long-horizon-planning-and-embodied-reasoning)
- [3. Memory, Skills, and Self-Improvement](#3-memory-skills-and-self-improvement)
- [4. Harnesses, Tools, and Orchestration](#4-harnesses-tools-and-orchestration)
- [5. World Models and Action-Conditioned Planning](#5-world-models-and-action-conditioned-planning)
- [6. Reward, Verification, and Process Assessment](#6-reward-verification-and-process-assessment)

## 1. Foundations and Generalist Policies

通用机器人策略、VLA 基础模型，以及把互联网知识、视觉语言知识或世界模型迁移到实体控制中的早期代表性工作。

- **[Do As I Can, Not As I Say: Grounding Language in Robotic Affordances](https://arxiv.org/abs/2204.01691)** · `2022 · CoRL`
  - Focus: 将语言模型的高层语义规划与机器人技能的 affordance/value grounding 结合，形成 SayCan 框架。
  - `Project:` [SayCan](https://say-can.github.io/)

- **[Diffusion Policy: Visuomotor Policy Learning via Action Diffusion](https://arxiv.org/abs/2303.04137)** · `2023 · RSS`
  - Focus: 使用条件扩散模型生成动作序列，并通过 receding-horizon 推理实现高质量 visuomotor control。
  - `Project:` [Diffusion Policy](https://diffusion-policy.cs.columbia.edu/)
  - `Code:` [real-stanford/diffusion_policy](https://github.com/real-stanford/diffusion_policy)

- **[RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control](https://arxiv.org/abs/2307.15818)** · `2023 · CoRL`
  - Focus: 将视觉语言模型中的互联网知识通过动作 token 化迁移到机器人控制。
  - `Project:` [RT-2](https://robotics-transformer2.github.io/)

- **[π₀: A Vision-Language-Action Flow Model for General Robot Control](https://arxiv.org/abs/2410.24164)** · `2024`
  - Focus: 以 flow matching/action expert 为核心，统一多种机器人形态和操作任务的通用控制。
  - `Project:` [π₀](https://www.pi.website/blog/pi0)
  - `Code:` [Physical-Intelligence/openpi](https://github.com/Physical-Intelligence/openpi)

- **[π₀.₅: a Vision-Language-Action Model with Open-World Generalization](https://arxiv.org/abs/2504.16054)** · `2025`
  - Focus: 通过异构数据和开放世界训练增强 VLA 对未见物体、场景与任务的泛化能力。
  - `Project:` [π₀.₅](https://pi.website/blog/pi05)
  - `Code:` [Physical-Intelligence/openpi](https://github.com/Physical-Intelligence/openpi)

- **[π₀.₆: a VLA That Learns From Experience](https://arxiv.org/abs/2511.14759)** · `2025`
  - Focus: 引入基于经验和反馈的持续改进，使 VLA 能够从实际执行结果中学习。
  - `Project:` [π₀.₆](https://pi.website/blog/pistar06)

- **[π₀.₇: a Steerable Generalist Robotic Foundation Model with Emergent Capabilities](https://arxiv.org/abs/2604.15483)** · `2026`
  - Focus: 研究可 steer 的通用机器人基础模型及其在规模化训练下出现的组合能力。
  - `Project:` [π₀.₇](https://pi.website/pi07)

- **[OpenVLA: An Open-Source Vision-Language-Action Model](https://arxiv.org/abs/2406.09246)** · `2024 · CoRL`
  - Focus: 基于 Open X-Embodiment 数据训练的开放 7B VLA，支持面向具体机器人和任务的微调。
  - `Project:` [OpenVLA](https://openvla.github.io/)
  - `Code:` [openvla/openvla](https://github.com/openvla/openvla)

- **[World Action Models are Zero-shot Policies](https://arxiv.org/abs/2602.15922)** · `2026`
  - Focus: DreamZero 将视频生成与动作预测结合为 world action model，探索零样本物理技能泛化。
  - `Project:` [DreamZero](https://dreamzero0.github.io/)
  - `Code:` [dreamzero0/dreamzero](https://github.com/dreamzero0/dreamzero)

- **[PaLM-E: An Embodied Multimodal Language Model](https://arxiv.org/abs/2303.03378)** · `2023 · ICML`
  - Focus: 将连续传感器观测编码为多模态输入，研究语言模型在具身任务中的感知、推理与控制。
  - `Project:` [PaLM-E](https://palm-e.github.io/)

## 2. Long-Horizon Planning and Embodied Reasoning

关注长时程任务分解、交互式推理、空间记忆、执行反馈和高层 agent 对机器人策略的组织。

- **[Towards Long-Horizon Agents: A Survey](https://openreview.net/pdf?id=HyhfhlbWGh)** · `2026`
  - Focus: 从基础模型、agent evolution、harness、优化方法和应用等角度系统梳理长时程 agent。
  - `Project:` [Long-Horizon Agents](https://long-horizon-agents.github.io/)
  - `Resources:` [Awesome-Long-Horizon-Agents](https://github.com/RUC-NLPIR/Awesome-Long-Horizon-Agents)

- **[DIRECT: When and Where Should You Allocate Test-Time Compute in Embodied Planners](https://arxiv.org/abs/2606.12402)** · `2026`
  - Focus: 自适应决定何时、何处以及分配多少 test-time compute，以提升具身规划的效率和可靠性。

- **[Learning from Trials and Errors: Reflective Test-Time Planning for Embodied LLMs](https://arxiv.org/abs/2602.21198)** · `2026`
  - Focus: 利用执行中的试错轨迹进行反思，在 test time 修正具身 LLM 的规划。
  - `Project:` [Reflective Test-Time Planning](https://reflective-test-time-planning.github.io/)
  - `Code:` [Reflective-Test-Time-Planning/Reflective-Test-Time-Planning](https://github.com/Reflective-Test-Time-Planning/Reflective-Test-Time-Planning)

- **[Agentic Robot: A Brain-Inspired Framework for Vision-Language-Action Models in Embodied Agents](https://arxiv.org/abs/2505.23450)** · `2025`
  - Focus: 以 planner、VLA policy 和 validator 构成闭环 agent，研究面向机器人任务的脑启发式组织方式。
  - `Project:` [Agentic Robot](https://agentic-robot.github.io/)
  - `Code:` [Agentic-Robot/agentic-robot](https://github.com/Agentic-Robot/agentic-robot)

- **[HoloAgent-0: A Unified Embodied Agent Framework with 3D Spatial Memory](https://arxiv.org/abs/2606.23565)** · `2026`
  - Focus: 使用统一 agent 框架和 3D spatial memory 支持跨时间、跨任务的空间推理与执行。
  - `Project:` [HoloAgent-0](https://horizonrobotics.github.io/robot_lab/holoagent)
  - `Code:` [HorizonRobotics/HoloAgent](https://github.com/HorizonRobotics/HoloAgent)

- **[Anticipation-VLA: Solving Long-Horizon Embodied Tasks via Anticipation-based Subgoal Generation](https://arxiv.org/abs/2605.01772)** · `2026`
  - Focus: 通过对未来状态和子目标进行 anticipation，降低长时程 VLA 执行中的规划跨度。

- **[Guide, Think, Act: Interactive Embodied Reasoning in Vision-Language-Action Models](https://arxiv.org/abs/2605.13632)** · `2026`
  - Focus: 将 guide、think 和 act 组织为交互式具身推理循环，让 VLA 在执行中获取并利用反馈。
  - `Project:` [Guide, Think, Act](https://signalispupupu.github.io/GTA-VLA_ProjPage/)

- **[Done, But Not Sure: Disentangling World Completion from Self-Termination in Embodied Agents](https://arxiv.org/abs/2605.08747)** · `2026`
  - Focus: 区分“世界状态已完成”和“agent 自己判断应终止”两个问题，减少错误的自终止。

- **[RoboAgent: Chaining Basic Capabilities for Embodied Task Planning](https://arxiv.org/abs/2604.07774)** · `2026 · CVPR`
  - Focus: 将基础视觉语言能力链式组合，用于复杂具身任务规划。

- **[VIA: Visual Interface Agent for Robot Control](https://arxiv.org/abs/2607.11119)** · `2026`
  - Focus: 通过视觉界面和交互式 agent 把高层任务指令转化为机器人控制行为。

- **[ETA: A New Agentic Paradigm for Embodied Tasks](https://arxiv.org/abs/2608.03924)** · `2026`
  - Focus: 探索面向具身任务的 agentic execution 范式，将任务理解、规划与物理执行统一到可扩展流程中。
  - `Project:` [OpenETA](https://openmoss.ai/OpenETA/)
  - `Code:` [OpenMOSS/OpenETA](https://github.com/OpenMOSS/OpenETA)

## 3. Memory, Skills, and Self-Improvement

关注长期记忆、技能发现与复用、自动课程、在线适应，以及在少量或零人工示范下持续提升机器人能力。

- **[ABot-AgentOS: A General Robotic Agent OS with Lifelong Multi-modal Memory](https://arxiv.org/abs/2607.10350)** · `2026`
  - Focus: 以 agent operating system 统一多模态感知、任务执行和 lifelong memory，并面向长期机器人交互。
  - `Project:` [ABot-AgentOS](https://amap-cvlab.github.io/ABot-AgentOS)
  - `Code:` [amap-cvlab/ABot-AgentOS](https://github.com/amap-cvlab/ABot-AgentOS)

- **[EmbodiSkill: Skill-Aware Reflection for Self-Evolving Embodied Agents](https://arxiv.org/abs/2605.10332)** · `2026`
  - Focus: 将 skill-level reflection 引入具身 agent 的自演化过程，促进技能获取、诊断与改进。
  - `Code:` [air-embodied-brain/EmbodiSkill](https://github.com/air-embodied-brain/EmbodiSkill)

- **[EvoMemNav: Efficient Self-Evolving Fine-Grained Memory for Zero-Shot Embodied Navigation](https://arxiv.org/abs/2606.03509)** · `2026`
  - Focus: 构建细粒度、可自演化的视觉语义记忆，增强 zero-shot embodied navigation。

- **[RoboMemory: A Brain-inspired Multi-memory Agentic Framework for Lifelong Learning in Physical Embodied Systems](https://arxiv.org/abs/2508.01415)** · `2025`
  - Focus: 以多种互补记忆模拟脑启发式长期学习，支持物理系统中的 agentic lifelong learning。
  - `Project:` [RoboMemory](https://sp4595.github.io/robomemory/)

- **[ASPIRE: Agentic Skill Discovery for Robotics](https://arxiv.org/abs/2607.00272)** · `2026`
  - Focus: 通过 agentic exploration 和代码化策略发现机器人可复用技能。
  - `Project:` [ASPIRE](https://research.nvidia.com/labs/gear/aspire/)

- **[ENPIRE: Agentic Robot Policy Self-Improvement in the Real World](https://arxiv.org/abs/2606.19980)** · `2026`
  - Focus: 将真实世界机器人策略改进组织为可重复的 physical autoresearch loop。
  - `Project:` [ENPIRE](https://enpire-research.github.io/)

- **[InSight: Self-Guided Skill Acquisition via Steerable VLAs](https://arxiv.org/abs/2606.24884)** · `2026`
  - Focus: 利用可 steer 的 VLA 进行自引导技能获取和数据/策略迭代。
  - `Project:` [InSight](https://insight-vla.github.io/)
  - `Code:` [insight-vla/insight](https://github.com/insight-vla/insight)

- **[From Exploration to Reuse: An Embodied Agent Framework for Manipulation Skill Learning](https://openreview.net/pdf?id=VnBoiEkZt2)** · `2026 · MARS Workshop`
  - Focus: 将探索、控制器参数优化和技能记忆结合，推动操作技能从发现走向复用。

- **[Playful Agentic Robot Learning](https://arxiv.org/abs/2606.19419)** · `2026`
  - Focus: 通过 self-directed play 产生交互经验，并沉淀可调用的机器人技能库。
  - `Project:` [Playful Agentic Robot Learning](https://playful-rats.github.io/)
  - `Code:` [Playful-RATs/RATs](https://github.com/Playful-RATs/RATs)

- **[Practice Makes Policies: Bootstrapping and Consolidating Robotic Capabilities from Zero Human Demonstrations](https://arxiv.org/abs/2607.26809)** · `2026`
  - Focus: HERO 从零人工示范开始，通过自主练习 bootstrapping 并 consolidation 机器人策略能力。
  - `Project:` [HERO](https://hero-agent.github.io/)

- **[Self-Improving Embodied Foundation Models](https://arxiv.org/abs/2509.15155)** · `2025 · NeurIPS`
  - Focus: 研究具身基础模型如何利用自身生成的数据、反馈和训练循环持续改进。

- **[Agentic-VLA: Efficient Online Adaptation for Vision-Language-Action Models](https://arxiv.org/abs/2605.22896)** · `2026 · ICML`
  - Focus: 面向 VLA 的高效 online adaptation，通过 agentic 数据选择和更新降低适应成本。

- **[MEMENTO: Memory-Guided Memetic Code-as-Policy Evolution](https://arxiv.org/abs/2607.22832)** · `2026`
  - Focus: 用记忆引导 memetic search，对 code-as-policy 进行生成、变异、评估和保留。
  - `Code:` [sygkounas/MEMENTO](https://github.com/sygkounas/MEMENTO)

- **[SkillMemo: Expert-guided Skill Memory Framework for Compositional Embodied Manipulation](https://arxiv.org/abs/2608.05970)** · `2026`
  - Focus: 使用专家引导的技能记忆支持组合式具身操作。
  - `Project:` [SkillMemo](https://changyuanwang17.github.io/SkillMemo/)

- **[Skills in Weights, Memory in Code: Hybrid Learning for Memory-Dependent Robot Manipulation](https://arxiv.org/abs/2608.09410)** · `2026`
  - Focus: 以 HyMeS 混合存储学习到的技能和代码化记忆，处理依赖长期记忆的机器人操作。

- **[SEED: Self-Evolving On-Policy Distillation for Agentic Reinforcement Learning](https://arxiv.org/abs/2607.14777)** · `2026`
  - Focus: 将 hindsight skills 与 on-policy distillation 结合，实现 agentic reinforcement learning 的自演化。
  - `Project:` [SEED](https://jinyangwu.github.io/seed/)
  - `Code:` [jinyangwu/SEED](https://github.com/jinyangwu/SEED)

- **[LEACL: LLM-Enhanced Automatic Curriculum Learning for Reinforcement Learning in Long-Horizon Manipulation Tasks](https://arxiv.org/abs/2607.23515)** · `2026`
  - Focus: 使用 LLM 自动生成和调整课程，提升长时程操作任务中的强化学习效率。

## 4. Harnesses, Tools, and Orchestration

关注 agent harness、工具调用、代码生成、策略编排、跨 embodiment 协作，以及把冻结策略组织成可靠长时程系统的基础设施。

- **[Code as Policies: Language Model Programs for Embodied Control](https://arxiv.org/abs/2209.07753)** · `2022`
  - Focus: 让语言模型生成可执行的 Python/程序化策略，把语言指令编译为具身控制流程。
  - `Project:` [Code as Policies](https://code-as-policies.github.io/)
  - `Code:` [google-research/code_as_policies](https://github.com/google-research/google-research/tree/master/code_as_policies)

- **[Harness VLA: Steering Frozen VLAs into Reliable Manipulation Primitives via Memory-Guided Agents](https://arxiv.org/abs/2607.08448)** · `2026`
  - Focus: 将冻结 VLA 作为可调用 primitive，通过记忆引导的 agent 进行重试、纠错和可靠性提升。
  - `Project:` [Harness VLA](https://harnessvla.github.io/)

- **[EmbodiedClaw: Conversational Workflow Execution for Embodied AI Development](https://arxiv.org/abs/2604.13800)** · `2026`
  - Focus: 以对话式 workflow 执行具身 AI 的开发、实验和部署任务。

- **[PhyAgentOS: A Self-Evolving Operating System for Embodied Agents with Decoupled Cognitive Planning and Physical Execution](https://arxiv.org/abs/2607.16636)** · `2026`
  - Focus: 解耦认知规划与物理执行，提供具身 agent 的运行时、验证和自演化操作系统。
  - `Project:` [PhyAgentOS](https://phy-agent-os.net/)
  - `Code:` [PhyAgentOS/PhyAgentOS](https://github.com/PhyAgentOS/PhyAgentOS)

- **[RoboClaw: An Agentic Framework for Scalable Long-Horizon Robotic Tasks](https://arxiv.org/abs/2603.11558)** · `2026`
  - Focus: 面向可扩展长时程机器人任务的 agentic framework，强调任务组织、执行与反馈闭环。

- **[GaP: A Graph-as-Policy Multi-Agent Self-Learning Harness for Variational Automation Tasks](https://arxiv.org/abs/2607.05369)** · `2026`
  - Focus: 用 typed graph-as-policy 组织多 agent 编程、仿真 rehearsal 与自动化任务的自学习。
  - `Project:` [GaP](https://graph-robots.github.io/gap)
  - `Code:` [graph-robots/graph-as-policy](https://github.com/graph-robots/graph-as-policy)

- **[CaP-X: A Framework for Benchmarking and Improving Coding Agents for Robot Manipulation](https://arxiv.org/abs/2603.22435)** · `2026 · ICML`
  - Focus: 为机器人操作 coding agents 提供 benchmark/gym，并研究基于反馈和强化学习的改进。
  - `Project:` [CaP-X](https://capgym.github.io/)
  - `Code:` [capgym/cap-x](https://github.com/capgym/cap-x)

- **[Guava: An Effective and Universal Harness for Embodied Manipulation](https://arxiv.org/abs/2606.18363)** · `2026`
  - Focus: 提炼通用 embodied manipulation harness 的关键组成，支持从复杂 agent 到紧凑策略的能力迁移。
  - `Project:` [Guava](https://guava-harness.github.io)

- **[VoLo: A Physical Orchestrator for Open-Vocabulary Long-Horizon Manipulation](https://arxiv.org/abs/2606.07723)** · `2026`
  - Focus: 作为 physical orchestrator 组织 VLA/WAM、工具、监控、暂停和重定向，执行开放词汇长时程操作。
  - `Project:` [VoLo](https://chicychen.github.io/VoLo/)
  - `Code:` [NVLabs/VoLoAgent](https://github.com/NVLabs/VoLoAgent)

- **[What Matters in Orchestrating Robot Policies: A Systematic Study of Hierarchical VLA Agents](https://arxiv.org/abs/2606.10267)** · `2026`
  - Focus: 系统研究层级 VLA agent 中的策略选择、编排、反馈和粒度等因素。

- **[Enabling Extensible Embodied Capabilities with Tools](https://arxiv.org/abs/2605.26637)** · `2026`
  - Focus: 通过工具接口扩展 embodied agent 的可用能力和任务覆盖范围。

- **[Exploratory, Communicative, and Deployable: Vision-Driven Embodied Agents for Open-World Mobile Manipulation](https://arxiv.org/abs/2607.13653)** · `2026`
  - Focus: 面向开放世界移动操作，统一探索、通信和可部署的视觉驱动 agent 能力。

- **[Addressing the Orchestration Gap in Generalist Robots via Physical Agency](https://arxiv.org/abs/2607.21725)** · `2026`
  - Focus: 从 physical agency 出发分析通用机器人从策略能力到可靠执行之间的 orchestration gap。

- **[RoboOS: A Hierarchical Embodied Framework for Cross-Embodiment and Multi-Agent Collaboration](https://arxiv.org/abs/2505.03673)** · `2025`
  - Focus: 以层级框架支持跨 embodiment 的技能调用和多 agent 协作。
  - `Project:` [RoboOS](https://flagopen.github.io/RoboOS/)
  - `Code:` [FlagOpen/RoboOS](https://github.com/FlagOpen/RoboOS)

- **[RoboOS-NeXT: A Unified Memory-based Framework for Lifelong, Scalable, and Robust Multi-Robot Collaboration](https://arxiv.org/abs/2510.26536)** · `2025`
  - Focus: 以统一记忆框架支持长期、可扩展且鲁棒的多机器人协作。
  - `Project:` [RoboOS](https://flagopen.github.io/RoboOS/)

- **[Zetta ζ: An Efficient Closed-Loop Embodied Harness for Self-Evolving Physical Intelligence](https://arxiv.org/abs/2608.16590)** · `2026`
  - Focus: 构建高效闭环 embodied harness，通过 critic、恢复和反馈实现物理智能自演化。
  - `Project:` [Zetta](https://air-embodied-brain.github.io/zetta)

- **[Thea: Towards the Harness of Embodied Agents](https://arxiv.org/abs/2608.11246)** · `2026`
  - Focus: 研究具身 agent harness 的工具、场景图、执行状态和退出码验证机制。
  - `Project:` [Thea](https://eit-hai.github.io/thea)
  - `Code:` [EIT-HAI/Thea](https://github.com/EIT-HAI/Thea)

- **[RoboBRIDGE: A Modular Framework for Bridging Policies to Robust Real-World Robotic Agents](https://arxiv.org/abs/2607.27881)** · `2026`
  - Focus: 以模块化的 monitor、perceptor、planner、controller 和 interface 将策略桥接到真实世界 agent。

- **[HarnessWAM: Bridging Prediction and Deliberation in World Action Models](https://arxiv.org/abs/2608.09516)** · `2026`
  - Focus: 在 world action model 中连接快速预测与审慎 deliberation，提升执行时的决策可靠性。

## 5. World Models and Action-Conditioned Planning

关注动作条件世界模型、未来状态想象和基于世界模型的 test-time planning。

- **[RISE: Self-Improving Robot Policy with Compositional World Model](https://arxiv.org/abs/2602.11075)** · `2026`
  - Focus: 使用 compositional world model 和进度价值估计进行想象式规划，支持机器人策略自改进。
  - `Project:` [RISE](https://opendrivelab.com/RISE)
  - `Code:` [OpenDriveLab/RISE](https://github.com/OpenDriveLab/RISE)

- **[τ₀-VLA: a Hierarchical Robot Foundation Model with World-Model-Guided Test-Time Computation](https://tau0-vla.github.io/tau0-vla.pdf)** · `2026`
  - Focus: 采用层级机器人基础模型，并使用世界模型指导 test-time computation 分配。
  - `Project:` [τ₀-VLA](https://tau0-vla.github.io/)
  - `Code:` [sii-research/tau-0-vla](https://github.com/sii-research/tau-0-vla)

- **[World Action Planner: Generalizable Decision-Making with Action-Conditioned World Models](https://arxiv.org/abs/2607.27599)** · `2026`
  - Focus: 通过 action-conditioned world model 进行可泛化决策和未来轨迹规划。
  - `Project:` [World Action Planner](https://worldactionplanner.github.io/)
  - `Code:` [XiangchengZhang/world-action-planner](https://github.com/XiangchengZhang/world-action-planner)

- **[RoboReact: Agentic Skill Distillation from Generated Egocentric Videos for Generalizable Whole-Body Manipulation](https://arxiv.org/abs/2608.03387)** · `2026`
  - Focus: 从生成的第一视角视频中蒸馏 agentic skills，增强全身操作的泛化能力。
  - `Project:` [RoboReact](https://roboreact.github.io/)

## 6. Reward, Verification, and Process Assessment

关注机器人轨迹的过程级评价、视觉语言奖励、失败驱动的 dense reward 和通用验证器。

- **[LLM-as-a-Verifier: A General-Purpose Verification Framework](https://arxiv.org/abs/2607.05391)** · `2026`
  - Focus: 使用 LLM/VLM 对复杂任务过程和结果进行通用验证，支持 agent 训练和部署时的反馈。
  - `Project:` [LLM-as-a-Verifier](https://llm-as-a-verifier.com/)
  - `Code:` [llm-as-a-verifier/llm-as-a-verifier](https://github.com/llm-as-a-verifier/llm-as-a-verifier)

- **[RoboReward: General-Purpose Vision-Language Reward Models for Robotics](https://arxiv.org/abs/2601.00675)** · `2026`
  - Focus: 构建通用视觉语言奖励模型，为多种机器人任务提供可迁移的 reward signal。
  - `Resources:` [RoboReward-Bench](https://crfm.stanford.edu/helm/robo-reward-bench)

- **[DenseReward: Dense Reward Learning via Failure Synthesis for Robotic Manipulation](https://arxiv.org/abs/2607.13033)** · `2026`
  - Focus: 通过失败轨迹合成学习 dense reward，改善机器人操作中的稀疏反馈问题。
  - `Project:` [DenseReward](https://dense-reward.github.io/)

- **[PRM-as-a-Judge 1.5: A Toolkit for Robot Process Assessment](https://arxiv.org/abs/2608.14284)** · `2026`
  - Focus: 将 process reward model 用作 robot process judge，对操作过程进行细粒度评估。
  - `Project:` [PRM-as-a-Judge](https://prm-as-a-judge.github.io)

## Link and Maintenance Policy

- 每篇论文只保留一个主论文入口；优先级为 `arXiv > 官方 OpenReview/出版页面 > 官方论文 PDF`。
- `Project` 指论文作者或官方组织维护的项目主页；`Code` 指能够确认与论文直接对应的公开代码仓库；`Resources` 指 benchmark、数据或相关资源，不等同于论文实现代码。
- 新增论文时请放入最贴近其主要贡献的一个分类，保留论文标题、年份和主论文链接，并尽量补充官方项目主页与代码链接。
- 若论文后来出现正式出版版本，可在原有主链接旁补充会议或期刊链接，但不应删除已有的 arXiv 入口。
