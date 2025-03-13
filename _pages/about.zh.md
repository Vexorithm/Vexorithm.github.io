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

<span class='anchor' id='关于我'></span>

# 关于我
大家好！我目前是南京信息工程大学人工智能学院的一名本科在读学生，有幸师从[许沛澜](https://scholar.google.ca/citations?hl=zh-CN&user=MYTn5zYAAAAJ "许沛澜")。

我的研究重点包括进化计算、LLM推理、多智能体框架以及各类LLM应用研究。多篇论文已投稿至人工智能领域的顶级期刊和会议（如ACM Transactions、IJCAI、ACL等），我的代表作"Density-Assisted Evolutionary Dynamic Multimodal Optimization"已被ACM TELO接收。

目前，我在[上海人工智能实验室](https://www.shlab.org.cn/ "上海人工智能实验室")实习，以及我的mentor是[苏锐](https://scholar.google.ca/citations?hl=zh-CN&authuser=2&user=tLLmRBwAAAAJ "苏锐")。同时，我在东京大学担任研究助理，与[赵新杰](https://scholar.google.com/citations?hl=zh-CN&user=_l5fPvEAAAAJ "赵新杰")教授密切合作。

我很荣幸能够以**Kaggle Expert**的身份获得LLM竞赛的两枚银牌。此外，我连续两年（2023年、2024年）在[IEEE CEC动态环境多最优解竞赛](http://mi.hitsz.edu.cn/activities/smode_cec2023/index.html)中获得冠军，并在蓝桥杯中获得全国一等奖。

我正在积极寻求学术合作机会，欢迎通过以下邮箱与我联系：<auraithm@gmail.com>（个人邮箱）或 <evonexusx@gmail.com>。

---

<span class='anchor' id='news'></span>
# 🔥 最新动态
- *2025.03*: &nbsp;🎉🎉 论文"Density-Assisted Evolutionary Dynamic Multimodal Optimization"被**ACM Transactions on Evolutionary Learning and Optimization**接收。
- *2025.03*: &nbsp;🎉🎉 在Kaggle竞赛"LLMs - You Can't Please Them All"中获得银牌。

---

<span class='anchor' id='honors-and-awards'></span>
# 🎖 荣誉与奖项
- *2025.03* 在Kaggle竞赛**"LLMs - You Can't Please Them All"**中获得银牌。
- *2024.07* 在**IEEE CEC 2024动态环境多最优解竞赛**中获得冠军。
- *2024.06* 在蓝桥杯中获得全国一等奖。
- *2024.04* 在Kaggle竞赛**"LLM Prompt Recovery"**中获得银牌。
- *2023.07* 在**IEEE CEC 2023动态环境多最优解竞赛**中获得冠军。

---

<span class='anchor' id='publications'></span>
# 📝 论文
- **Density-Assisted Evolutionary Dynamic Multimodal Optimization**, **Ying Zhu**, Peilan Xu, Jiahao Huang, Xin Lin, Wenjian Luo, **ACM TELO**.
- **[GRATR: Zero-Shot Evidence Graph Retrieval-Augmented Trustworthiness Reasoning](https://arxiv.org/abs/2408.12333)**, **Ying Zhu\***, Shengchang Li\*, Ziqian Kong, Qiang Yang, Peilan Xu, **IJCAI 2025 (Under the second reviewing phase)**.
- **[Narrative-Driven Travel Planning: Geocultural-Grounded Script Generation with Evolutionary Itinerary Optimization](https://arxiv.org/abs/2502.14456)**, Ran Ding\*, Ziyu Zhang\*, **Ying Zhu\***, Ziqian Kong, Peilan Xu, **ACL 2025 (Under Review)**.
- **ReAgent: Reversible Multi-Agent Reasoning for Knowledge-Enhanced Multi-Hop QA**, Zhao Xinjie, Fan Gao, Rui Yang, Yingjian Chen, Yuyang Wang, **Ying Zhu**, Jiacheng Tang, Irene Li, **ACL 2025 (Under Review)**.
- **Adaptive Interruption and Trust-Weighted Voting for Secure Multi-Agent Collaboration in Complex Question Answering**, **Ying Zhu\***, Zhao Xinjie, Irene Li, **arXiv**.

---

<span class='anchor' id='research-overview'></span>
# 💬 研究概述

## **Density-Assisted Evolutionary Dynamic Multimodal Optimization**

**作者：** **Ying Zhu**, Peilan Xu, Jiahao Huang, Xin Lin, Wenjian Luo

**期刊：ACM Transactions on Evolutionary Learning and Optimization**（已接收）

**代码：<https://github.com/EvoNexusX/2023ZhuDAEA>**


<div style="text-align: center; margin: 0 auto; max-width: 50%;">
    <div class="badge">ACM TELO</div>
    <img src='{{ site.baseurl }}/images/Density_00.png' alt="sym" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
</div>
 
### 摘要
动态多模态优化问题（DMMOPs）要求算法能够在连续环境变化之间的有限计算资源限制下，快速定位和跟踪多个最优解。主要挑战在于控制种群多样性以促进有效探索。在本文中，我们研究了利用当前和历史种群中的密度信息来增强探索。首先，对于每个活跃子种群，我们基于同时活跃的子种群分布构建密度景观，并根据密度和适应度值建立候选解之间的支配关系，引导该子种群探索低密度有前景区域。然后，对于每个已收敛的子种群，我们基于历史上已灭绝的子种群分布构建密度景观，引导该子种群在低密度未开发区域重新启动。最后，我们开发了一个全面的密度辅助进化算法（DAEA）框架，包含密度辅助搜索和重启，并结合初始化。此外，我们采用预测和记忆策略来增强DAEA在动态环境中的性能。值得注意的是，该算法依赖外部监控器来检测环境变化并触发动态响应策略。DAEA在CEC'2022动态多模态优化基准套件上进行了测试，并与多个最先进的动态多模态优化算法进行了比较。实验结果表明DAEA在处理DMMOPs方面具有竞争力。

---

## **[GRATR: Zero-Shot Evidence Graph Retrieval-Augmented Trustworthiness Reasoning](https://arxiv.org/abs/2408.12333)**

**作者：** **Ying Zhu\***, Shengchang Li\*, Ziqian Kong, Qiang Yang, Peilan Xu

**会议：IJCAI 2025**（二审阶段）

**代码：<https://github.com/EvoNexusX/2025ZhuGRATR>**


<div style="text-align: center; margin: 0 auto; max-width: 100%;">
    <div class="badge">IJCAI 2025</div>
    <img src='/images/fig2_00.png' alt="sym" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
</div>
 
### 摘要

可信度推理旨在使不完整信息多人游戏中的智能体能够识别潜在的盟友和对手，从而增强决策能力。在本文中，我们提出了图检索增强的可信度推理（GRATR）框架，该框架从游戏环境中检索可观察的证据，为大型语言模型（LLMs）的决策提供信息，无需额外训练，使其成为一种零样本方法。在GRATR框架中，智能体首先观察其他玩家的行为并评估由此产生的玩家间信任变化，构建相应的可信度图。在决策过程中，智能体执行多跳检索来评估对特定目标的可信度，其中从多个可信来源检索证据链以形成全面评估。在多人游戏《狼人杀》中的实验表明，GRATR优于其他方法，与基线方法相比，推理准确率提高了50.5%，幻觉减少了30.6%。此外，在美国大选期间的Twitter推文数据集上测试时，GRATR的准确率比基线方法高出10.4%，突出了其在意图分析等实际应用中的潜力。
 
---

## **[Narrative-Driven Travel Planning: Geocultural-Grounded Script Generation with Evolutionary Itinerary Optimization](https://arxiv.org/abs/2502.14456)**

**作者：**  Ran Ding\*, Ziyu Zhang\*, **Ying Zhu\***, Ziqian Kong, Peilan Xu

**会议：ACL 2025**（审稿中）

**代码：<https://github.com/EvoNexusX/2025DingNarrativeGuide>**


<div style="text-align: center; margin: 0 auto; max-width: 100%;">
    <div class="badge">ACL 2025</div>
    <img src='/images/3.png' alt="sym" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
</div>
 
### 摘要

为了提升游客的体验和沉浸感，本文提出了一个叙事驱动的旅行规划框架NarrativeGuide，为旅行者生成基于地理文化的叙事脚本，提供新颖的角色扮演式旅程体验。在初始阶段，NarrativeGuide为城市内的景点构建知识图谱，然后基于知识图谱配置世界观、角色设定和背景介绍。利用这个基础，结合知识图谱为每个景点生成独立的场景单元。在行程规划阶段，NarrativeGuide将叙事驱动的旅行规划建模为优化问题，利用遗传算法（GA）优化行程。在评估候选行程之前，为每对相邻景点生成过渡脚本，与场景单元一起形成完整脚本。然后使用脚本连贯性、旅行时间和景点评分的加权和作为适应度值来更新候选解集。在中国南京和扬州、法国巴黎和德国柏林四个城市的实验结果表明，在叙事连贯性和文化契合度方面有显著提升，同时旅行时间显著减少，访问景点质量提高。我们的研究表明，引入外部进化优化有效解决了大型语言模型在旅行规划中的局限性。

---

## **ReAgent: Reversible Multi-Agent Reasoning for Knowledge-Enhanced Multi-Hop QA**

**作者：**  Zhao Xinjie, Fan Gao, Rui Yang, Yingjian Chen, Yuyang Wang, **Ying Zhu**, Jiacheng Tang, Irene Li

**会议：ACL 2025**（审稿中）

<div style="text-align: center; margin: 0 auto; max-width: 100%;">
    <div class="badge">ACL 2025</div>
    <img src='/images/4.png' alt="sym" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
</div>
 
### 摘要

大型语言模型（LLMs）的最新进展通过直接链式思维（CoT）推理显著改进了多跳问答（QA）。然而，CoT的不可逆性导致错误累积，使得在多跳推理中难以纠正错误。本文介绍了ReAgent：一个具有显式回溯机制的可逆多智能体协作框架，实现可逆多跳推理。通过结合基于文本的检索、信息聚合和验证，我们的系统能够在推理过程中检测和纠正错误，产生更稳健和可解释的QA结果。该框架和实验为未来容错QA系统的工作奠定了基础。在三个基准上的实证评估表明ReAgent的有效性，与基线模型相比平均提高了约6%。

---

## **Adaptive Interruption and Trust-Weighted Voting for Secure Multi-Agent Collaboration in Complex Question Answering**

**作者：** **Ying Zhu\***, Zhao Xinjie, Irene Li
 
### 摘要

复杂问答通常需要对多个信息源进行推理并整合不同形式的知识。然而，依赖单一链式思维可能导致错误传播，系统仍然容易受到恶意或误导性输入的影响。在本文中，我们提出了一个增强的多智能体框架，引入细粒度中断（"断点"）机制和动态信任加权投票策略，以提高多跳QA的稳健性和可解释性。我们的方法整合了贝叶斯启发的智能体可信度更新、逐段答案生成和基于数学的中断策略，以限制错误传播。我们描述了系统的理论基础和实践工作流程，然后展示了中断触发、加权投票和多智能体协作如何协同产生更准确和安全的答案。在基准QA数据集上的实验证实了正确性、稳定性和可解释性的显著改进，显示出在对抗性或高风险环境中更广泛应用的潜力。
 
---

# 📖 教育经历
<span class='anchor' id='educations'></span>
- *2022.09 - 2025.03（至今）*, 南京信息工程大学人工智能学院。

---

# 💻 实习经历
<span class='anchor' id='internships'></span>
- *2024.10 - 2025.03（至今）*, 实习, 上海人工智能实验室（[Shanghai AI Lab](https://www.shlab.org.cn/ "上海人工智能实验室")）, 中国。
- *2024.11 - 2025.03（至今）*, 研究助理, 东京大学, 日本。
- *2025.01 - 2025.03（至今）*, 研究助理, 云南省红河州蒙自市科技局, 中国**（国有企业）**。
