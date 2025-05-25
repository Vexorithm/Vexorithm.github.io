---
permalink: /zh/
title: ""
excerpt: ""
author_profile: true
lang: zh
redirect_from: 
  - /zh/about/
  - /zh/about.html
---
 
{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

# 关于我
大家好！我目前是南京信息工程大学人工智能学院的一名本科在读学生，由[许沛澜](https://scholar.google.ca/citations?hl=zh-CN&user=MYTn5zYAAAAJ "许沛澜")导师指导。

我的研究重点包括Evolutionary Computation、LLM Reasoning、Multi-Agent Frameworks以及各类LLM应用研究。多篇论文已投稿至人工智能领域的顶级期刊和会议（如ACM Transactions、IJCAI、ACL等），我的代表作"Density-Assisted Evolutionary Dynamic Multimodal Optimization"已被ACM TELO接收。

目前，我在[Shanghai AI Lab](https://www.shlab.org.cn/ "上海人工智能实验室")实习，我的mentor是[苏锐](https://scholar.google.ca/citations?hl=zh-CN&authuser=2&user=tLLmRBwAAAAJ "苏锐")。在这之前，我在东京大学担任Research Assistant，并与[赵新杰](https://scholar.google.com/citations?hl=zh-CN&user=_l5fPvEAAAAJ "赵新杰")密切合作。

我很荣幸能够获得Kaggle LLM竞赛的两枚银牌并获得**Kaggle Expert**称号。此外，我连续两年（2023年、2024年）在[IEEE CEC Competition on Seeking Multiple Optima in Dynamic Environments](http://mi.hitsz.edu.cn/activities/smode_cec2023/index.html)中获得冠军，并在蓝桥杯算法竞赛中获得全国一等奖。

我正在积极寻求学术合作机会，欢迎通过以下邮箱与我联系：<auraithm@gmail.com>（个人邮箱）或 <evonexusx@gmail.com>。

---

<span class='anchor' id='-news'></span>
# 🔥 最新动态
- *2025.03*: &nbsp;🎉🎉 论文"Density-Assisted Evolutionary Dynamic Multimodal Optimization"被**ACM Transactions on Evolutionary Learning and Optimization**接收。
- *2025.03*: &nbsp;🎉🎉 在Kaggle竞赛"LLMs - You Can't Please Them All"中获得银牌。

---

<span class='anchor' id='-honors-and-awards'></span>
# 🎖 荣誉与奖项
- *2025.03* 在Kaggle竞赛**"LLMs - You Can't Please Them All"**中获得银牌。
- *2024.07* 在**IEEE CEC 2024 Competition on Seeking Multiple Optima in Dynamic Environments**中获得冠军。
- *2024.06* 在蓝桥杯中获得全国一等奖。
- *2024.04* 在Kaggle竞赛**"LLM Prompt Recovery"**中获得银牌。
- *2023.07* 在**IEEE CEC 2023 Competition on Seeking Multiple Optima in Dynamic Environments**中获得冠军。

---

<span class='anchor' id='-publications'></span>
# 📝 论文
- **[Density-Assisted Evolutionary Dynamic Multimodal Optimization](https://dl.acm.org/doi/pdf/10.1145/3723171)**, **Ying Zhu**, Peilan Xu, Jiahao Huang, Xin Lin, Wenjian Luo, **ACM TELO**.
- **[Swarm Intelligence Enhanced Reasoning: A Density-Driven Framework for LLM-Based Multi-Agent Optimization]**, **Ying Zhu**, Peilan Xu, Jiahao Huang, Xin Lin, Wenjian Luo, **ACM TELO**.
- **[GRATR: Zero-Shot Evidence Graph Retrieval-Augmented Trustworthiness Reasoning](https://arxiv.org/abs/2408.12333)**, **Ying Zhu\***, Shengchang Li\*, Ziqian Kong, Qiang Yang, Peilan Xu, **EMNLP 2025 (Under review.)**.
- **[Narrative-Driven Travel Planning: Geocultural-Grounded Script Generation with Evolutionary Itinerary Optimization](https://arxiv.org/abs/2502.14456)**, Ran Ding\*, Ziyu Zhang\*, **Ying Zhu\***, Ziqian Kong, Peilan Xu, **ACL 2025 (Under Review)**
---

<span class='anchor' id='-research-overview'></span>
# 💬 研究概述

## **[Density-Assisted Evolutionary Dynamic Multimodal Optimization](https://dl.acm.org/doi/pdf/10.1145/3723171)**

**作者：** **Ying Zhu**, Peilan Xu, Jiahao Huang, Xin Lin, Wenjian Luo

**期刊：ACM Transactions on Evolutionary Learning and Optimization**（已接收）

**代码：<https://github.com/EvoNexusX/2023ZhuDAEA>**


<div style="text-align: center; margin: 0 auto; max-width: 50%;">
    <div class="badge">ACM TELO</div>
    <img src='{{ site.baseurl }}/images/Density_00.png' alt="sym" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
</div>
 
### 摘要
Dynamic Multimodal Optimization Problems (DMMOPs)要求算法能够在连续环境变化之间的有限计算资源限制下，快速定位和跟踪多个最优解。主要挑战在于控制种群多样性以促进有效探索。在本文中，我们研究了利用当前和历史种群中的密度信息来增强探索。首先，对于每个活跃子种群，我们基于同时活跃的子种群分布构建密度景观，并根据密度和适应度值建立候选解之间的支配关系，引导该子种群探索低密度有前景区域。然后，对于每个已收敛的子种群，我们基于历史上已灭绝的子种群分布构建密度景观，引导该子种群在低密度未开发区域重新启动。最后，我们开发了一个全面的Density-Assisted Evolutionary Algorithm (DAEA)框架，包含密度辅助搜索和重启，并结合初始化。此外，我们采用预测和记忆策略来增强DAEA在动态环境中的性能。值得注意的是，该算法依赖外部监控器来检测环境变化并触发动态响应策略。DAEA在CEC'2022 Dynamic Multimodal Optimization基准套件上进行了测试，并与多个state-of-the-art动态多峰优化算法进行了比较。实验结果表明DAEA在处理DMMOPs方面具有竞争力。

---

## **[Swarm Intelligence Enhanced Reasoning: A Density-Driven Framework for LLM-Based Multi-Agent Optimization]

**作者：** **Ying Zhu\***, Heng Zhou, Rui Su, Peiqin Zhuang, LEI BAI 
**会议：NeurIPS 2025**（在投）

<div style="text-align: center; margin: 0 auto; max-width: 100%;">
    <div class="badge">NeurIPS 2025</div>
    <img src='/images/fig2_00.png' alt="sym" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
</div>
 
### 摘要

最近，人们提出了许多方法来进一步丰富大型语言模型(LLMs)在推理场景中的复杂问题解决能力，比如思维链(Chain-of-Thought, CoT)提示和多智能体辩论(Multi-Agent Debate, MAD)。然而，由于缺乏寻找最优解的能力，这些方法可能在解决复杂问题时失败。群智能(Swarm Intelligence)在传统优化问题领域一直是一个强大的工具。为此，我们提出通过引入一种新颖的基于智能体的群智能(Agent-based Swarm Intelligence, ASI)范式，将群智能整合到推理过程中。在这个范式中，我们将LLM推理表述为一个优化问题，并使用群智能方案来指导一组基于LLM的智能体协作搜索最优解。为了避免群智能陷入局部最优，我们进一步开发了一个群智能增强推理(Swarm Intelligence Enhancing Reasoning, SIER)框架，该框架采用密度驱动策略来增强推理能力。具体来说，我们提出使用核密度估计和非支配排序来同时优化解决方案的质量和多样性。在这种情况下，SIER通过扩展推理路径的多样性来有效增强解空间探索。此外，我们还使用步骤级质量评估来帮助智能体通过纠正低质量的中间步骤来提高解决方案质量。然后，我们使用质量阈值来动态控制探索的终止和候选步骤的选择，从而实现更灵活和高效的推理过程。我们在七个广泛使用的数学推理基准测试上进行了大量实验，包括MATH-500、MMLU-STEM等。正如预期的那样，我们的方法在性能上始终优于CoT方法和现有的奖励引导方法，特别是在复杂问题上。这证明了我们提出的利用群智能来增强推理的方法的有效性。

 
---

## **[GRATR: Zero-Shot Evidence Graph Retrieval-Augmented Trustworthiness Reasoning](https://arxiv.org/abs/2408.12333)**

**作者：** **Ying Zhu\***, Shengchang Li\*, Ziqian Kong, Qiang Yang, Peilan Xu

**会议：EMNLP 2025**（在投）

**代码：<https://github.com/EvoNexusX/2025ZhuGRATR>**


<div style="text-align: center; margin: 0 auto; max-width: 100%;">
    <div class="badge">EMNLP 2025</div>
    <img src='/images/fig2_00.png' alt="sym" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
</div>
 
### 摘要

Trustworthiness Reasoning旨在使不完整信息多人游戏中的智能体能够识别潜在的盟友和对手，从而增强决策能力。在本文中，我们提出了Graph Retrieval-Augmented Trustworthiness Reasoning (GRATR)框架，该框架从游戏环境中检索可观察的证据，为Large Language Models (LLMs)的决策提供信息，无需额外训练，使其成为一种zero-shot方法。在GRATR框架中，智能体首先观察其他玩家的行为并评估由此产生的玩家间信任变化，构建相应的trustworthiness graph。在决策过程中，智能体执行multi-hop retrieval来评估对特定目标的可信度，其中从多个可信来源检索evidence chains以形成全面评估。在多人游戏《Werewolf》中的实验表明，GRATR优于其他方法，与baseline方法相比，reasoning accuracy提高了50.5%，hallucination减少了30.6%。此外，在美国大选期间的Twitter推文数据集上测试时，GRATR的accuracy比baseline方法高出10.4%，突出了其在intent analysis等实际应用中的潜力。
 
---

## **[Narrative-Driven Travel Planning: Geocultural-Grounded Script Generation with Evolutionary Itinerary Optimization](https://arxiv.org/abs/2502.14456)**

**作者：**  Ran Ding\*, Ziyu Zhang\*, **Ying Zhu\***, Ziqian Kong, Peilan Xu

**会议：EMNLP 2025**（在投）

**代码：<https://github.com/EvoNexusX/2025DingNarrativeGuide>**


<div style="text-align: center; margin: 0 auto; max-width: 100%;">
    <div class="badge">ACL 2025</div>
    <img src='/images/3.png' alt="sym" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
</div>
 
### 摘要

为了提升游客的体验和沉浸感，本文提出了一个narrative-driven travel planning框架NarrativeGuide，为旅行者生成基于geocultural的narrative script，提供新颖的role-playing式旅程体验。在初始阶段，NarrativeGuide为城市内的景点构建knowledge graph，然后基于knowledge graph配置worldview、character setting和exposition。利用这个基础，结合knowledge graph为每个景点生成独立的scene unit。在行程规划阶段，NarrativeGuide将narrative-driven travel planning建模为optimization problem，利用Genetic Algorithm (GA)优化行程。在评估candidate itinerary之前，为每对相邻景点生成transition script，与scene unit一起形成完整script。然后使用script coherence、travel time和attraction scores的加权和作为fitness value来更新candidate solution set。在中国南京和扬州、法国巴黎和德国柏林四个城市的实验结果表明，在narrative coherence和cultural fit方面有显著提升，同时travel time显著减少，访问景点quality提高。我们的研究表明，引入外部evolutionary optimization有效解决了Large Language Models在travel planning中的limitations。

---

<!-- 
## **ReAgent: Reversible Multi-Agent Reasoning for Knowledge-Enhanced Multi-Hop QA** (During RA at the University of Tokyo)

**作者：**  Zhao Xinjie, Fan Gao, Rui Yang, Yingjian Chen, Yuyang Wang, **Ying Zhu**, Jiacheng Tang, Irene Li

**会议：ACL 2025**（在投）

<div style="text-align: center; margin: 0 auto; max-width: 100%;">
    <div class="badge">ACL 2025</div>
    <img src='/images/4.png' alt="sym" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
</div>
 
### 摘要

Large Language Models (LLMs)的最新进展通过直接Chain-of-Thought (CoT) reasoning显著改进了Multi-Hop Question Answering (QA)。然而，CoT的不可逆性导致error accumulation，使得在multi-hop reasoning中难以纠正错误。本文介绍了ReAgent：一个具有显式backtracking机制的Reversible Multi-Agent collaborative框架，实现reversible multi-hop reasoning。通过结合基于文本的retrieval、information aggregation和validation，我们的系统能够在reasoning过程中检测和纠正错误，产生更robust和interpretable的QA结果。该框架和实验为未来error-tolerant QA系统的工作奠定了基础。在三个benchmark上的empirical evaluation表明ReAgent的有效性，与baseline models相比平均提高了约6%。

---

## **Adaptive Interruption and Trust-Weighted Voting for Secure Multi-Agent Collaboration in Complex Question Answering** (During RA at the University of Tokyo)

**作者：** **Ying Zhu\***, Zhao Xinjie, Irene Li

**状态：** 已完成，待投中。
 
### 摘要

Complex Question Answering通常需要对多个信息源进行reasoning并整合不同形式的knowledge。然而，依赖单一chain-of-thought可能导致error propagation，系统仍然容易受到malicious或misleading inputs的影响。在本文中，我们提出了一个enhanced multi-agent framework，引入fine-grained interruption ("breakpoint")机制和dynamic trust-weighted voting策略，以提高multi-hop QA的robustness和explainability。我们的方法整合了Bayesian-inspired agent credibility updates、segment-by-segment answer generation和mathematically grounded interruption strategy，以限制error propagation。我们描述了系统的theoretical underpinnings和practical workflow，然后展示了interruption triggers、weighted voting和multi-agent collaboration如何协同产生更accurate和secure的答案。在benchmark QA datasets上的experiments证实了correctness、stability和interpretability的显著改进，显示出在adversarial或high-stakes环境中更广泛应用的潜力。
 
--- -->

# 📖 教育经历
<span class='anchor' id='-educations'></span>
- *2022.09 - 2025.03（至今）*, Nanjing University of Information Science and Technology, School of Artificial Intelligence.

---

# 💻 实习经历
<span class='anchor' id='-internships'></span>
- *2025.01 - 2025.04（至今）*, 实习生, 上海人工智能实验室 ([Shanghai AI Lab](https://www.shlab.org.cn/ "上海人工智能实验室")), 中国。
- *2025.09 - 2025.02*, 研究助理, 东京大学, 日本。