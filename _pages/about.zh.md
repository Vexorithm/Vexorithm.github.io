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
大家好！我目前是南京信息工程大学人工智能学院的一名本科在读学生，有幸得到[许沛澜](https://scholar.google.ca/citations?hl=zh-CN&user=MYTn5zYAAAAJ "许沛澜")导师的指导， 主要进行进化算法、群体智能的研究。

目前，我在[上海人工智能实验室](https://www.shlab.org.cn/ "上海人工智能实验室")实习，由[苏锐](https://scholar.google.ca/citations?hl=zh-CN&authuser=2&user=tLLmRBwAAAAJ "苏锐")和[白磊](https://scholar.google.com/citations?user=sakOO04AAAAJ&hl=en&oi=ao "白磊")老师指导。我的研究重点包括LLM推理、多智能体框架、群智能以及各类LLM应用研究。多篇论文已投稿至人工智能领域的顶级期刊和会议（如ACM Transactions、ACL、NeurIPS、EMNLP等），我的代表作"Density-Assisted Evolutionary Dynamic Multimodal Optimization"已被ACM TELO接收。

我很荣幸能够获得**Kaggle Expert**称号，在LLM竞赛中获得两枚银牌。此外，我连续两年（2023年、2024年）在[IEEE CEC Competition on Seeking Multiple Optima in Dynamic Environments](http://mi.hitsz.edu.cn/activities/smode_cec2023/index.html)中获得冠军，并在蓝桥杯算法竞赛中获得全国一等奖。

我正在积极寻求学术合作机会，欢迎通过以下邮箱与我联系：<auraithm@gmail.com>。

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
- ## **[Density-Assisted Evolutionary Dynamic Multimodal Optimization](https://dl.acm.org/doi/pdf/10.1145/3723171)**, **Ying Zhu**, Peilan Xu, Jiahao Huang, Xin Lin, Wenjian Luo, **ACM TELO**.
- **[Swarm Intelligence Enhanced Reasoning: A Density-Driven Framework for LLM-Based Multi-Agent Optimization](https://arxiv.org/abs/2505.17115)**, **Ying Zhu\***, Heng Zhou, Rui Su, Peiqin Zhuang, Lei Bai **NeurIPS 2025 (Under Review)**.
- **[GRATR: Zero-Shot Evidence Graph Retrieval-Augmented Trustworthiness Reasoning](https://arxiv.org/abs/2408.12333)**, **Ying Zhu\***, Shengchang Li\*, Ziqian Kong, Qiang Yang, Peilan Xu, **EMNLP 2025 (Under Review)**.
- **[Narrative-Driven Travel Planning: Geocultural-Grounded Script Generation with Evolutionary Itinerary Optimization](https://arxiv.org/abs/2502.14456)**, Ziyu Zhang\*, Ran Ding\*, **Ying Zhu\***, Ziqian Kong, Peilan Xu

---

<span class='anchor' id='-research-overview'></span>
# 💬 研究概述（“*”表明共同贡献）

## **[Density-Assisted Evolutionary Dynamic Multimodal Optimization](https://dl.acm.org/doi/pdf/10.1145/3723171)**

**作者：** **Ying Zhu**, Peilan Xu, Jiahao Huang, Xin Lin, Wenjian Luo

**期刊：ACM Transactions on Evolutionary Learning and Optimization**（已接收）

**代码：<https://github.com/EvoNexusX/2023ZhuDAEA>**


<div style="text-align: center; margin: 0 auto; max-width: 50%;">
    <div class="badge">ACM TELO</div>
    <img src='/images/Density_00.png' alt="sym" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
</div>
 
### 摘要
动态多峰优化问题(DMMOPs)要求算法能够在时间上快速定位和跟踪多个最优解。主要挑战在于控制种群多样性以促进有效探索，所有这些都在连续环境变化之间有限计算资源的限制内。在本文中，我们研究了利用来自当前和历史种群的密度信息来增强探索。首先，对于每个活跃子种群，我们基于同时活跃子种群的分布构建密度景观，并根据密度和适应度值建立候选解之间的支配关系，引导该子种群探索低密度有前景区域。然后，对于每个已收敛的子种群，我们基于历史上已灭绝的子种群分布构建密度景观，引导该子种群在低密度未开发区域重新启动。最后，我们开发了一个全面的密度辅助进化算法(DAEA)框架，包含密度辅助搜索和重启，并结合初始化。此外，我们采用预测和记忆策略来增强DAEA在动态环境中的性能。值得注意的是，该算法依赖外部监控器来检测环境变化并触发动态响应策略。DAEA在CEC'2022动态多峰优化基准套件上进行了测试，并与多个最先进的动态多峰优化算法进行了比较。实验结果表明DAEA在处理DMMOPs方面具有竞争力。

---

## **[Swarm Intelligence Enhanced Reasoning: A Density-Driven Framework for LLM-Based Multi-Agent Optimization](https://arxiv.org/abs/2505.17115)**

**作者：** **Ying Zhu\***, Heng Zhou, Rui Su, Peiqin Zhuang, Lei Bai 

**会议：NeurIPS 2025**（在投）

<div style="text-align: center; margin: 0 auto; max-width: 100%;">
    <div class="badge">NeurIPS 2025</div>
    <img src='/images/SIER.png' alt="sym" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
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

可信度推理旨在使不完整信息多人游戏中的智能体能够识别潜在的盟友和对手，从而增强决策能力。在本文中，我们提出了图检索增强可信度推理(GRATR)框架，该框架从游戏环境中检索可观察的证据，为大型语言模型(LLMs)的决策提供信息，无需额外训练，使其成为一种零样本方法。在GRATR框架中，智能体首先观察其他玩家的行为并评估由此产生的玩家间信任变化，构建相应的可信度图。在决策过程中，智能体执行多跳检索来评估对特定目标的可信度，其中从多个可信来源检索证据链以形成全面评估。在多人游戏《狼人杀》中的实验表明，GRATR优于其他方法，与基线方法相比，推理准确率提高了50.5%，幻觉减少了30.6%。此外，在美国大选期间的Twitter推文数据集上测试时，GRATR的准确率比基线方法高出10.4%，突出了其在意图分析等实际应用中的潜力。

---

## **[Narrative-Driven Travel Planning: Geocultural-Grounded Script Generation with Evolutionary Itinerary Optimization](https://arxiv.org/abs/2502.14456)**

**作者：** Ziyu Zhang\*, **Ying Zhu\***, Ziqian Kong, Peilan Xu

**会议：EMNLP 2025**（在投）

**代码：<https://github.com/EvoNexusX/2025DingNarrativeGuide>**


<div style="text-align: center; margin: 0 auto; max-width: 100%;">
    <div class="badge">EMNLP 2025</div>
    <img src='/images/3.png' alt="sym" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
</div>
 
### 摘要

为了提升游客的体验和沉浸感，本文提出了一个叙事驱动旅行规划框架NarrativeGuide，为旅行者生成基于地理文化的叙事脚本，提供新颖的角色扮演式旅程体验。在初始阶段，NarrativeGuide为城市内的景点构建知识图谱，然后基于知识图谱配置世界观、角色设定和背景介绍。利用这个基础，结合知识图谱为每个景点生成独立的场景单元。在行程规划阶段，NarrativeGuide将叙事驱动旅行规划建模为优化问题，利用遗传算法(GA)优化行程。在评估候选行程之前，为每对相邻景点生成过渡脚本，与场景单元一起形成完整脚本。然后使用脚本连贯性、旅行时间和景点评分的加权和作为适应度值来更新候选解集。在我们的实验中，我们整合了TravelPlanner基准来系统评估NarrativeGuide在复杂约束下的规划能力。此外，我们还评估了其在叙事连贯性和文化契合度方面的表现。结果表明，NarrativeGuide在行程规划和脚本生成方面都表现出强大的能力。

---

## **[Black-Sheep Agent: Semantic Sabotage in Multi-Agent Language Games]**
**Authors:** Zhao Xinjie*,  **Ying Zhu\***, Jiacheng Tang

**Conference: EMNLP 2025** (Under Review)


<div style="text-align: center; margin: 0 auto; max-width: 100%;">
    <div class="badge">EMNLP 2025</div>
    <img src='/images/5.png' alt="sym" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
</div>
 
### Abstract

大型语言模型越来越多地被用于公共决策，从参与式预算到在线慈善拍卖。然而，现有的防御措施主要针对单次提示注入，而忽视了更隐蔽的*多轮、多智能体*劝说形式。我们引入了*语义“黑羊”智能体*的概念：一个恶意参与者，系统地利用语言学原理操纵集体廉价谈话，从而扭曲博弈均衡。为了形式化和基准化这一威胁，我们将**语义破坏**定义为廉价谈话的Stackelberg竞赛，并提出*BlackSheep–Game*，这是第一个将四种语言哲学攻击向量——(*i*) 预设注入，(*ii*) 词汇-收益歧义，(*iii*) Gricean准则反转，和(*iv*) 言语行为重映射——应用于五个经典社会困境（迭代公共物品、Vickrey拍卖、协调、Stackelberg分配和社区预算谈判）的框架。即使是单个黑羊智能体（占参与者的5%）也能将纳什均衡偏移高达41%，并在绕过最先进的毒性和越狱过滤器的同时，侵蚀整体福利18-46%。基于稳健的多智能体学习和语义平滑的见解，我们进一步提出了一种可部署的防护措施，能够在安全性与实时可用性之间取得平衡。我们的结果为可信赖的LLM集体铺平了道路，并强调了防御语言级别对手以保护公民决策的紧迫性。

---

# 📖 教育经历
<span class='anchor' id='-educations'></span>
- *2022.09 - 2025.06（至今）*, 南京信息工程大学人工智能学院。

---

# 💻 实习经历
<span class='anchor' id='-internships'></span>
- *2025.01 - 2025.06（至今）*, 实习生, 上海人工智能实验室 ([Shanghai AI Lab](https://www.shlab.org.cn/ "上海人工智能实验室")), 中国。
