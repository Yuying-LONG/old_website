---
layout: default
title: Publications
---

<!-- 1. 这里是样式代码，直接保留在 md 文件里即可 -->
<style>
.pub-item {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    margin-bottom: 40px; /* 每篇论文之间的间距 */
    border-bottom: 1px solid #eee;
    padding-bottom: 20px;
}

.pub-img {
    flex: 0 0 250px; /* 图片宽度固定为 250px */
    width: 250px;
}

.pub-img img {
    width: 100%;
    border-radius: 5px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    object-fit: cover;
}

.pub-content {
    flex: 1; /* 文字部分占据剩余空间 */
    min-width: 300px;
}

.pub-title {
    font-size: 1.1em;
    font-weight: bold;
    margin-bottom: 8px;
    line-height: 1.4;
}

.pub-authors {
    color: #555;
    margin-bottom: 5px;
    font-style: italic;
}

.pub-venue {
    color: #222;
    margin-bottom: 10px;
    font-weight: 500;
}

.pub-abstract {
    font-size: 0.9em;
    color: #666;
    background-color: #f9f9f9;
    padding: 10px;
    border-radius: 5px;
    line-height: 1.5;
    margin-top: 10px;
}

/* 手机端适配：图片变大，上下排列 */
@media (max-width: 768px) {
    .pub-item { flex-direction: column; }
    .pub-img { width: 100%; flex: auto; }
}
</style>

<h1 id="publications">Publications</h1>
<h2 style="margin: 30px 0px 20px;">Selected Papers</h2>
<p>(**"*" for the corresponding author**)</p>

<!-- ================= 论文 [11] 开始 ================= -->
<div class="pub-item">
  <!-- 左侧图片：请修改 src 为你的图片路径 -->
  <div class="pub-img">
    <img src="/assets/img/11.jpg" alt="Paper Image">
  </div>
  
  <!-- 右侧内容 -->
  <div class="pub-content">
    <div class="pub-title">
      <a href="https://ieeexplore.ieee.org/document/11172291">[11] Learning-based Heterogeneous Autonomous Vehicles Scheduling for On-demand Last-mile Transportation</a>
    </div>
    
    <div class="pub-authors">
      Y. Liu, B. Xie, <b>Y. Long</b>, J. Chen, & G. Xu*
    </div>
    
    <div class="pub-venue">
      IEEE Transactions on Automation Science and Engineering (2025)
    </div>
    
    <!-- 摘要区域 -->
    <div class="pub-abstract">
      <b>Abstract:</b> Last-mile transportation, a critical component of public transit within integrated urban mobility systems, plays a pivotal role in promoting sustainability and requires immediate attention. However, due to the high real-time variability and uncertainties of last-mile travel demand, high passenger concurrency, and dispersed destinations, existing last-mile transportation systems often encounter significant challenges. These challenges include resource shortages and congestion during peak hours, as well as high operational costs and excessive passenger waiting times during off-peak periods. With the rapid development and widespread adoption of autonomous vehicles, which are characterized by centralized control and flexible scheduling, this study proposes leveraging heterogeneous autonomous vehicles to address these challenges. Specifically, a mixed-integer programming model is developed to maximize the service provider’s profit by considering fare profit, passenger waiting time penalties, and operating costs. To enable real-time decision-making, then an attention-based deep reinforcement learning algorithm is introduced. This algorithm incorporates two decoder mechanisms for vehicle selection and passenger allocation in the scheduling of heterogeneous autonomous vehicles. This involves dynamically selecting vehicles from a heterogeneous fleet based on passenger demand using an attention mechanism, optimizing efficiency in serving last-mile travelers. Extensive numerical experiments and a real-world case study across various datasets demonstrate that the proposed service model and algorithm effectively solve the scheduling problem while meeting the demands of on-demand last-mile transportation. Furthermore, these innovations contribute to reducing fleet carbon emissions and advancing sustainable urban transportation. Note to Practitioners—Last-mile transportation systems face critical challenges: overcrowded vehicles during peak hours, high costs due to underused resources in off-peak periods, and passenger dissatisfaction from long wait times. These issues hinder sustainable urban mobility and strain transit operators’ budgets. This work addresses these problems by deploying heterogeneous autonomous vehicle fleets with varying sizes and capabilities for last-mile transportation. The proposed system dynamically assigns vehicles to passengers based on real-time demand, optimizing efficiency while reducing operational costs. For transit operators, this approach balances fare revenue with penalties for passenger delays, ensuring profitability even during fluctuating demand. Cities adopting shared autonomous vehicle services can benefit from reduced congestion and lower carbon emissions, aligning with sustainability goals. Our experiments validate that the method improves service reliability and fleet utilization across demand scenarios. Implementing this solution requires integrating demand prediction tools with a centralized autonomous vehicle dispatch platform, compatible with existing mobility apps. Future extensions could adapt the system to mixed fleets (combining autonomous vehicles with traditional vehicles) or expand to multi-city networks. By addressing both economic and environmental needs, this framework offers a scalable path toward smarter, greener urban transportation.
    </div>
  </div>
</div>
<!-- ================= 论文 [11] 结束 ================= -->


<!-- ================= 论文 [10] 开始 ================= -->
<div class="pub-item">
  <div class="pub-img">
    <!-- 记得上传图片并修改这里的路径 -->
    <img src="/assets/img/10.jpg" alt="Paper Image">
  </div>
  
  <div class="pub-content">
    <div class="pub-title">
      <a href="https://www.sciencedirect.com/science/article/pii/S0957417424030859">[10] A matheuristic solution for efficient scheduling in dynamic truck-drone collaboration</a>
    </div>
    
    <div class="pub-authors">
      J. Zhao, <b>Y. Long</b>, B. Xie*, G. Xu, & Y. Liu
    </div>
    
    <div class="pub-venue">
      Expert Systems with Applications (2024)
    </div>
    
    <div class="pub-abstract">
      <b>Abstract:</b> Unmanned aerial vehicles (UAVs), or drones, have great potential for emergency response operations in areas with vulnerable road networks and infrastructure. However, the low battery capacity restricts their quick, cost-effective, and efficient aerial transportation capabilities. To overcome this drawback, hybrid systems that combine trucks and drones have emerged as a promising solution. Nevertheless, the fixed-binding mode between trucks and drones in most studies tends to impair efficiency by limiting drones’ operational flexibility. This paper investigates a dynamic truck–drone collaboration (DTDC) strategy for efficient and flexible emergency response. This strategy enables drones to dynamically change take-off and landing locations on different trucks, which is beneficial in emergency scenarios with common road network disruptions. Despite its advantages, the DTDC strategy introduces additional complexity to the scheduling problem, resulting in a time-consuming solution. To enhance solution efficiency and improve the application prospects of this strategy, we propose a matheuristic to decouple DTDC’s multiple synchronization constraints, separating the scheduling problem into three decision-making processes: demand allocation, truck routing, and drone scheduling. Additionally, two alternative matheuristic algorithms are designed to target accuracy and computing efficiency, respectively. The empirical results indicate that the proposed heuristics outperform the state-of-the-art solver and several metaheuristics. A sensitivity analysis confirms that improvements in drone endurance and the strategic reservation of drone parking slots on trucks can significantly improve the DTDC strategy’s performance.
    </div>
  </div>
</div>
<!-- ================= 论文 [10] 结束 ================= -->
