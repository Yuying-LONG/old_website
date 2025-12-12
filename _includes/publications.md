---
layout: default
title: Publications
---

<!-- ================== CSS 样式区域 ================== -->
<style>
/* 1. 卡片整体容器 */
.pub-card {
    display: flex;              /* 左右布局 */
    height: 260px;              /* 【关键】固定高度，你可以调整这个数字 */
    border: 1px solid #e5e5e5;  /* 边框颜色 */
    background: #fff;
    margin-bottom: 30px;        /* 卡片之间的间距 */
    border-radius: 8px;         /* 圆角 */
    overflow: hidden;           /* 保证圆角不被内部元素溢出遮挡 */
    box-shadow: 0 4px 6px rgba(0,0,0,0.05); /* 轻微阴影 */
}

/* 2. 左侧：信息区域 */
.pub-left {
    flex: 1;                    /* 占据剩余宽度 */
    padding: 20px;              /* 内边距 */
    display: flex;
    flex-direction: column;     /* 上下排列：Title -> Meta -> Abstract */
    overflow: hidden;           /* 防止溢出 */
}

/* 3. 右侧：图片区域 */
.pub-right {
    flex: 0 0 300px;            /* 【关键】固定图片区域宽度，可调整 */
    position: relative;
}

.pub-right img {
    width: 100%;
    height: 100%;
    object-fit: cover;          /* 核心：保持比例裁切图片，填满右侧区域 */
    object-position: center;    /* 图片居中 */
}

/* 4. 各个元素的字体样式 */
.pub-title {
    margin: 0 0 8px 0;
    font-size: 1.1rem;
    line-height: 1.3;
    font-weight: bold;
}

.pub-title a {
    text-decoration: none;
    color: #333;
}
.pub-title a:hover {
    color: #007bff;             /* 鼠标悬停颜色 */
}

.pub-meta {
    font-size: 0.9rem;
    color: #666;
    margin-bottom: 10px;
    font-style: italic;
    flex-shrink: 0;             /* 防止作者栏被压缩 */
}

.pub-abstract {
    font-size: 0.85rem;
    color: #555;
    line-height: 1.5;
    background: #f9f9f9;
    padding: 10px;
    border-radius: 4px;
    
    /* 【核心功能】超出高度滚动 */
    flex: 1;                    /* 占满剩余高度 */
    overflow-y: auto;           /* 内容多了就出现滚动条 */
}

/* 美化滚动条（Webkit内核浏览器） */
.pub-abstract::-webkit-scrollbar {
    width: 6px;
}
.pub-abstract::-webkit-scrollbar-thumb {
    background-color: #ddd;
    border-radius: 3px;
}

/* 5. 手机端适配：取消固定高度，变成上下排列 */
@media (max-width: 768px) {
    .pub-card {
        height: auto;           /* 手机上自动高度 */
        flex-direction: column-reverse; /* 图片在上面(row-reverse)或下面(column)？这里设为column */
    }
    .pub-right {
        flex: auto;
        height: 200px;          /* 手机上图片的高度 */
        width: 100%;
    }
    .pub-abstract {
        overflow-y: visible;    /* 手机上不滚动，全部显示 */
    }
}
</style>

<h1 id="publications">Publications</h1>
<h2 style="margin: 30px 0px 20px;">Selected Papers</h2>
<p>(**"*" for the corresponding author**)</p>


<!-- ================= 论文 [11] ================= -->
<div class="pub-card">
    <!-- 左侧：文字信息 -->
    <div class="pub-left">
        <h3 class="pub-title">
            <a href="https://ieeexplore.ieee.org/document/11172291">[11] Learning-based Heterogeneous Autonomous Vehicles Scheduling for On-demand Last-mile Transportation</a>
        </h3>
        
        <div class="pub-meta">
            Y. Liu, B. Xie, <b>Y. Long</b>, J. Chen, & G. Xu*. 
            <br>
            <i>IEEE Transactions on Automation Science and Engineering (2025)</i>
        </div>
        
        <div class="pub-abstract">
            <b>Abstract:</b> Last-mile transportation, a critical component of public transit within integrated urban mobility systems, plays a pivotal role in promoting sustainability and requires immediate attention. However, due to the high real-time variability and uncertainties of last-mile travel demand, high passenger concurrency, and dispersed destinations, existing last-mile transportation systems often encounter significant challenges. These challenges include resource shortages and congestion during peak hours, as well as high operational costs and excessive passenger waiting times during off-peak periods. With the rapid development and widespread adoption of autonomous vehicles, which are characterized by centralized control and flexible scheduling, this study proposes leveraging heterogeneous autonomous vehicles to address these challenges. Specifically, a mixed-integer programming model is developed to maximize the service provider’s profit by considering fare profit, passenger waiting time penalties, and operating costs. To enable real-time decision-making, then an attention-based deep reinforcement learning algorithm is introduced. This algorithm incorporates two decoder mechanisms for vehicle selection and passenger allocation in the scheduling of heterogeneous autonomous vehicles. This involves dynamically selecting vehicles from a heterogeneous fleet based on passenger demand using an attention mechanism, optimizing efficiency in serving last-mile travelers. Extensive numerical experiments and a real-world case study across various datasets demonstrate that the proposed service model and algorithm effectively solve the scheduling problem while meeting the demands of on-demand last-mile transportation. Furthermore, these innovations contribute to reducing fleet carbon emissions and advancing sustainable urban transportation. Note to Practitioners—Last-mile transportation systems face critical challenges: overcrowded vehicles during peak hours, high costs due to underused resources in off-peak periods, and passenger dissatisfaction from long wait times. These issues hinder sustainable urban mobility and strain transit operators’ budgets. This work addresses these problems by deploying heterogeneous autonomous vehicle fleets with varying sizes and capabilities for last-mile transportation. The proposed system dynamically assigns vehicles to passengers based on real-time demand, optimizing efficiency while reducing operational costs. For transit operators, this approach balances fare revenue with penalties for passenger delays, ensuring profitability even during fluctuating demand. Cities adopting shared autonomous vehicle services can benefit from reduced congestion and lower carbon emissions, aligning with sustainability goals. Our experiments validate that the method improves service reliability and fleet utilization across demand scenarios. Implementing this solution requires integrating demand prediction tools with a centralized autonomous vehicle dispatch platform, compatible with existing mobility apps. Future extensions could adapt the system to mixed fleets (combining autonomous vehicles with traditional vehicles) or expand to multi-city networks. By addressing both economic and environmental needs, this framework offers a scalable path toward smarter, greener urban transportation.
        </div>
    </div>

    <!-- 右侧：图片 -->
    <div class="pub-right">
        <!-- 请替换图片路径 -->
        <img src="/assets/img/11.jpg" alt="Paper Image">
    </div>
</div>


<!-- ================= 论文 [10] ================= -->
<div class="pub-card">
    <div class="pub-left">
        <h3 class="pub-title">
            <a href="https://www.sciencedirect.com/science/article/pii/S0957417424030859">[10] A matheuristic solution for efficient scheduling in dynamic truck-drone collaboration</a>
        </h3>
        
        <div class="pub-meta">
            J. Zhao, <b>Y. Long</b>, B. Xie*, G. Xu, & Y. Liu.
            <br>
            <i>Expert Systems with Applications (2024)</i>
        </div>
        
        <div class="pub-abstract">
            <b>Abstract:</b> Unmanned aerial vehicles (UAVs), or drones, have great potential for emergency response operations in areas with vulnerable road networks and infrastructure. However, the low battery capacity restricts their quick, cost-effective, and efficient aerial transportation capabilities. To overcome this drawback, hybrid systems that combine trucks and drones have emerged as a promising solution. Nevertheless, the fixed-binding mode between trucks and drones in most studies tends to impair efficiency by limiting drones’ operational flexibility. This paper investigates a dynamic truck–drone collaboration (DTDC) strategy for efficient and flexible emergency response. This strategy enables drones to dynamically change take-off and landing locations on different trucks, which is beneficial in emergency scenarios with common road network disruptions. Despite its advantages, the DTDC strategy introduces additional complexity to the scheduling problem, resulting in a time-consuming solution. To enhance solution efficiency and improve the application prospects of this strategy, we propose a matheuristic to decouple DTDC’s multiple synchronization constraints, separating the scheduling problem into three decision-making processes: demand allocation, truck routing, and drone scheduling. Additionally, two alternative matheuristic algorithms are designed to target accuracy and computing efficiency, respectively. The empirical results indicate that the proposed heuristics outperform the state-of-the-art solver and several metaheuristics. A sensitivity analysis confirms that improvements in drone endurance and the strategic reservation of drone parking slots on trucks can significantly improve the DTDC strategy’s performance.
        </div>
    </div>

    <div class="pub-right">
        <!-- 请替换图片路径 -->
        <img src="/assets/img/10.jpg" alt="Paper Image">
    </div>
</div>
