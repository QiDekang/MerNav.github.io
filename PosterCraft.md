---
layout: postercraft
permalink: /
title: MerNav
extra_css:
  - /assets/css/postercraft.css
extra_js:
  - /assets/js/postercraft.js
---

<!-- 顶部浮动demo图片 - 更新版本 -->
<div class="floating-demos">

    <div class="demo-right">
        <img src="images/janusvln/fig1.png" alt="AI Generated Poster Demo 2">
    </div>
    
</div>

<div class="hero">
    <div class="hero-content">

        <div class="title-logo-section">
            <h1 class="hero-title">MerNav</h1>
            <!--
            <div class="inline-logo">
                <div class="logo-glow-effect-inline"></div>
                <img src="images/janusvln/logo.png" alt="JanusVLN Logo" class="main-logo-inline">
                <div class="logo-sparkles-inline">
                    <span class="logo-sparkle logo-sparkle-1">✨</span>
                    <span class="logo-sparkle logo-sparkle-2">🌟</span>
                    <span class="logo-sparkle logo-sparkle-3">⭐️</span>
                </div>
            </div>
            -->
        </div>
        
        <!-- Paper信息 - 紧凑布局 -->
        <div class="paper-info-compact">
            <h3 class="paper-title-main">
                MerNav: A Highly Generalizable Memory-Execute-Review Framework for Zero-Shot Object Goal Navigation
            </h3>
            <a href="https://arxiv.org/pdf/2602.05467" target="_blank" rel="noopener noreferrer">
                <div class="paper-badge-fancy">📄 Research Paper</div>
            </a>
        </div>
        
        <!-- 作者信息 -->
        <div class="authors-section">
            <p class="authors">
                <span class="author"><a href="https://scholar.google.com/citations?user=fOU1xMAAAAAJ&hl=zh-CN&oi=ao">Dekang Qi</a><sup>1</sup></span>,
                <span class="author"><a href="https://scholar.google.com/citations?user=91lbdPcAAAAJ&hl=zh-CN">Shuang Zeng</a><sup>1,2</sup></span>,
                <span class="author"><a href="https://scholar.google.com/citations?user=5OnPBVYAAAAJ&hl=zh-CN&oi=ao">Xinyuan Chang</a><sup>1</sup></span>,
                <span class="author"><a href="https://scholar.google.com/citations?hl=zh-CN&user=_X4MQ-gAAAAJ">Feng Xiong</a><sup>1</sup></span>,
                <span class="author"><a>Shichao Xie</a><sup>1</sup></span>,
                <span class="author"><a>Xiaolong Wu</a><sup>1</sup></span>,
                <span class="author"><a>Mu Xu</a><sup>1</sup></span>,
            </p>
            <p class="affiliations">
                <sup>1</sup>Amap, Alibaba Group,
                <sup>2</sup>Xi'an Jiaotong University<br>
            </p>
        </div>
        
        <!-- 论文链接 - 增强版 -->
        <!--
        <div class="paper-links-enhanced">
            <a href="https://arxiv.org/abs/2602.05467" class="paper-link-fancy arxiv-link" target="_blank">
                <div class="link-icon-fancy">📚</div>
                <span>arXiv</span>
                <div class="link-shine"></div>
            </a>
            
            <a href="https://github.com/MIV-XJTU/JanusVLN" class="paper-link-fancy github-link" target="_blank">
                <div class="link-icon-fancy">💻</div>
                <span>GitHub</span>
                <div class="link-shine"></div>
            </a>
            <a href="https://www.modelscope.cn/models/misstl/JanusVLN_Base" class="paper-link-fancy huggingface-link" target="_blank">
                <div class="link-icon-fancy">🤗</div>
                <span>Model (JanusVLN_Base)</span>
                <div class="link-shine"></div>
            </a>
            <a href="https://www.modelscope.cn/models/misstl/JanusVLN_Extra" class="paper-link-fancy demo-link" target="_blank">
                <div class="link-icon-fancy">🚀</div>
                <span>Model (JanusVLN_Extra)</span>
                <div class="link-shine"></div>
            </a>
            <a href="https://www.modelscope.cn/datasets/misstl/JanusVLN_Trajectory_Data" class="paper-link-fancy dataset-link" target="_blank">
                <div class="link-icon-fancy">📊</div>
                <span>Datasets</span>
                <div class="link-shine"></div>
            </a>
            
            <a href="https://www.youtube.com/watch?v=U0IpLJOu48Y" class="paper-link-fancy video-link" target="_blank">
                <div class="link-icon-fancy">🎬</div>
                <span>Demo Video</span>
                <div class="link-shine"></div>
            </a>
            
        </div>
        -->
    </div>
</div>

<!-- Abstract Section -->
<div class="abstract-section">
    <div class="abstract-container">
        <h2 class="abstract-title">Abstract</h2>
        <p class="abstract-text">
            Visual Language Navigation (VLN) is one of the fundamental capabilities for embodied intelligence and a critical challenge that urgently needs to be addressed. However, existing methods are still unsatisfactory in terms of both success rate (SR) and generalization: Supervised Fine-Tuning (SFT) approaches typically achieve higher SR, while Training-Free (TF) approaches often generalize better, but it is difficult to obtain both simultaneously. To this end, we propose a Memory-Execute-Review framework. It consists of three parts: a hierarchical memory module for providing information support, an execute module for routine decision-making and actions, and a review module for handling abnormal situations and correcting behavior. We validated the effectiveness of this framework on the Object Goal Navigation task. Across 4 datasets, our average SR achieved absolute improvements of 7% and 5% compared to all baseline methods under TF and Zero-Shot (ZS) settings, respectively. On the most commonly used HM3D_v0.1 and the more challenging open vocabulary dataset HM3D_OVON, the SR improved by 8% and 6%, under ZS settings. Furthermore, on the MP3D and HM3D_OVON datasets, our method not only outperformed all TF methods but also surpassed all SFT methods, achieving comprehensive leadership in both SR (5% and 2%) and generalization. Additionally, we deployed the MerNav model on the humanoid robot and conducted experiments in the real world. The project address is: https://qidekang.github.io/MerNav.github.io/
        </p>
    </div>
</div>

<div class="what-is-section" id="what-is">
    <div class="what-is-container">
        <h2 class="what-is-title">Approach</h2>

        <!-- Approach图片 -->
            <div class="approach-image-container">
                <img src="images/janusvln/fig2.png" alt="JanusVLN Framework Approach" class="approach-image">
            </div>

        
        <!-- 新的横向布局 -->
        <div class="horizontal-demo-container">
            <div class="demo-row">
                <div class="demo-row-background">
                    <div class="demo-label-horizontal">
                        
                        <span class="label-text">The framework of MerNav. Memory-Execute-Review. The Memory module provides priors and informational support for decision-making; under nominal conditions, task completion is handled by the Execute module. Meanwhile, the Review module continuously monitors the execution process from an independent perspective and, upon detecting
anomalies or deviations, triggers corresponding corrective modes to rectify behavior.</span>
                    </div>
                    
                </div>
            </div>
            

            
        </div>
    </div>
</div>

<!-- Dataset Showcase Section - Styled like Technical Overview -->
<div class="technical-overview-section" id="dataset-showcase">
    <div class="overview-container">
        <div class="overview-header">
            <h2 class="overview-title">Experiment</h2>

            <div class="approach-image-container">
                <img src="images/janusvln/results.jpg" alt="results" class="approach-image">
            </div>

            <div class="approach-image-container">
                <img src="images/janusvln/results2.jpg" alt="results" class="approach-image">
            </div>

            
        </div>

        
    </div>
</div>

<!-- 新增：Technical Overview Section - 全栏设计 -->
<div class="technical-overview-section" id="overview">
    <div class="overview-container">
        <div class="overview-header">
            <h2 class="overview-title">Real-World Visualization</h2>
        </div>
          <div class="overview-header">
            <h3 class="overview-title" style="font-size: 36px;">Real Case 1, Object Goal: Plants</h3>
        </div>
        <div style="display: flex; flex-wrap: wrap; gap: 10px; margin-top: 20px;">
            <img src="https://raw.githubusercontent.com/QiDekang/MerNav.github.io/main/images/real_case/palnt/plants.png" style="width: 98%;">
        </div>

         <iframe width="560" height="315" src="https://www.youtube.com/embed/iSkDKXJyQ7Y?si=LfrWYhd0VVDyAEPv" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
         <iframe width="560" height="315" src="https://www.youtube.com/embed/oWku_paSfw4?si=5J6UUsshcxE0-bH5" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


          <div class="overview-header" style="margin-top: 50px;">
            <h3 class="overview-title" style="font-size: 36px;">Real Case 2, Object Goal: Football</h3>
        </div>
        <div style="display: flex; flex-wrap: wrap; gap: 10px; margin-top: 20px;">
            <img src="https://raw.githubusercontent.com/QiDekang/MerNav.github.io/main/images/real_case/football/football.png" style="width: 98%;">
        </div>

         <iframe width="560" height="315" src="https://www.youtube.com/embed/m3Nt2KkMI48?si=VtmrM67qMBHyzMQg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
         <iframe width="560" height="315" src="https://www.youtube.com/embed/6Mcuh3PoCm0?si=kq_KCG4oCsUjZu1b" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

    </div>
</div>





<div class="technical-overview-section" id="overview">
    <div class="overview-container">
        <div class="overview-header">
            <h2 class="overview-title">BibTeX Citation</h2>
        </div>

        <div class="bibtex-container">
            <div class="bibtex-content">
                <pre class="bibtex-text">
                    @article{qi2026mernav,
                      title={MerNav: A Highly Generalizable Memory-Execute-Review Framework for Zero-Shot Object Goal Navigation},
                      author={Qi, Dekang and Zeng, Shuang and Chang, Xinyuan and Xiong, Feng and Xie, Shichao and Wu, Xiaolong and Xu, Mu},
                      journal={arXiv preprint arXiv:2602.05467},
                      year={2026}
                    }
                </pre>
                <button class="copy-button" onclick="copyBibtex()">
                    <span class="copy-icon">📋</span>
                    <span class="copy-text">Copy</span>
                </button>
            </div>
        </div>
        
    </div>
</div>




