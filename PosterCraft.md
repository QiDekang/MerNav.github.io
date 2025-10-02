---
layout: postercraft
permalink: /
title: JanusVLN
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
            <h1 class="hero-title">JanusVLN:</h1>
            <div class="inline-logo">
                <div class="logo-glow-effect-inline"></div>
                <img src="images/janusvln/logo.png" alt="JanusVLN Logo" class="main-logo-inline">
                <div class="logo-sparkles-inline">
                    <span class="logo-sparkle logo-sparkle-1">✨</span>
                    <span class="logo-sparkle logo-sparkle-2">🌟</span>
                    <span class="logo-sparkle logo-sparkle-3">⭐️</span>
                </div>
            </div>
        </div>
        
        <!-- Paper信息 - 紧凑布局 -->
        <div class="paper-info-compact">
            <h3 class="paper-title-main">
                Decoupling Semantics and Spatiality with Dual Implicit Memory for Vision-Language Navigation
            </h3>
            <a href="https://arxiv.org/pdf/2509.22548" target="_blank" rel="noopener noreferrer">
                <div class="paper-badge-fancy">📄 Research Paper</div>
            </a>
        </div>
        
        <!-- 作者信息 -->
        <div class="authors-section">
            <p class="authors">
                <span class="author"><a href="https://scholar.google.com/citations?user=91lbdPcAAAAJ&hl=zh-CN">Shuang Zeng</a><sup>1,2,*</sup></span>,
                <span class="author"><a href="https://scholar.google.com/citations?user=fOU1xMAAAAAJ&hl=zh-CN&oi=ao">Dekang Qi</a><sup>1</sup></span>,
                <span class="author"><a href="https://scholar.google.com/citations?user=5OnPBVYAAAAJ&hl=zh-CN&oi=ao">Xinyuan Chang</a><sup>1</sup></span>,
                <span class="author"><a href="https://scholar.google.com/citations?hl=zh-CN&user=_X4MQ-gAAAAJ">Feng Xiong</a><sup>1</sup></span>,
                <span class="author"><a>Shichao Xie</a><sup>1</sup></span>,
                <span class="author"><a>Xiaolong Wu</a><sup>1</sup></span>,
                <span class="author"><a>Shiyi Liang</a><sup>1,2</sup></span>,
                <span class="author"><a>Mu Xu</a><sup>1</sup></span>,
                <span class="author"><a href="https://scholar.google.com/citations?hl=zh-CN&user=KNyC5EUAAAAJ">Xing Wei</a><sup>2†</sup></span>
            </p>
            <p class="affiliations">
                <sup>1</sup>Amap, Alibaba Group,
                <sup>2</sup>Xi'an Jiaotong University<br>
                <img src="images/janusvln/amap.png" alt="Amap Logo" style="height: 50px; background-color: white; padding: 3px; border-radius: 3px; margin-top: 5px;">
                <img src="images/janusvln/xjtu.png" alt="XJTU Logo" style="height: 50px; background-color: white; padding: 3px; border-radius: 3px; margin-top: 5px;">
            </p>
        </div>
        
        <!-- 论文链接 - 增强版 -->
        <div class="paper-links-enhanced">
            <a href="https://arxiv.org/abs/2509.22548" class="paper-link-fancy arxiv-link" target="_blank">
                <div class="link-icon-fancy">📚</div>
                <span>arXiv</span>
                <div class="link-shine"></div>
            </a>
            <a href="https://github.com/MIV-XJTU/JanusVLN" class="paper-link-fancy github-link" target="_blank">
                <div class="link-icon-fancy">💻</div>
                <span>GitHub</span>
                <div class="link-shine"></div>
            </a>
            <a href="https://huggingface.co/PosterCraft/PosterCraft-v1_RL" class="paper-link-fancy huggingface-link" target="_blank">
                <div class="link-icon-fancy">🤗</div>
                <span>HuggingFace (Coming soon)</span>
                <div class="link-shine"></div>
            </a>
            <a href="https://huggingface.co/spaces/Ephemeral182/PosterCraft" class="paper-link-fancy demo-link" target="_blank">
                <div class="link-icon-fancy">🚀</div>
                <span>ModelScope (Coming soon)</span>
                <div class="link-shine"></div>
            </a>
            <a href="https://huggingface.co/PosterCraft" class="paper-link-fancy dataset-link" target="_blank">
                <div class="link-icon-fancy">📊</div>
                <span>Datasets (Coming soon)</span>
                <div class="link-shine"></div>
            </a>
            <a href="https://www.youtube.com/watch?v=U0IpLJOu48Y" class="paper-link-fancy video-link" target="_blank">
                <div class="link-icon-fancy">🎬</div>
                <span>Demo Video</span>
                <div class="link-shine"></div>
            </a>
        </div>
    </div>
</div>

<!-- Abstract Section -->
<div class="abstract-section">
    <div class="abstract-container">
        <h2 class="abstract-title">Abstract</h2>
        <p class="abstract-text">
            Vision-and-Language Navigation (VLN) requires an embodied agent to navigate through unseen environments, guided by natural language instructions and a continuous video stream. 
            Recent advances in VLN have been driven by the powerful semantic understanding of Multimodal Large Language Models (MLLMs). However, these methods typically rely on explicit semantic memory, such as building textual cognitive maps or storing historical visual frames. This type of method suffers from spatial information loss, computational redundancy, and memory bloat, which impede efficient navigation. 
            Inspired by the implicit scene representation in human navigation, analogous to the left brain's semantic understanding and the right brain's spatial cognition, we propose JanusVLN, a novel VLN framework featuring a dual implicit neural memory that models spatial-geometric and visual-semantic memory as separate, compact, and fixed-size neural representations.
            This framework first extends the MLLM to incorporate 3D prior knowledge from the spatial-geometric encoder, thereby enhancing the spatial reasoning capabilities of models based solely on RGB input.
            Then, the historical key-value (KV) caches from the spatial-geometric and visual-semantic encoders are constructed into a dual implicit memory. By retaining only the KVs of tokens in the initial and sliding window, redundant computation is avoided, enabling efficient incremental updates.
            Extensive experiments demonstrate that JanusVLN outperforms over 20 recent methods to achieve SOTA performance. For example, the success rate improves by 10.5-35.5 compared to methods using multiple data types as input and by 3.6-10.8 compared to methods using more RGB training data.
            This indicates that the proposed dual implicit neural memory, as a novel paradigm, explores promising new directions for future VLN research.
        </p>
    </div>
</div>

<!-- Video Showcase Section -->
<div class="video-showcase-section" id="video-showcase">
    <div class="video-showcase-container">
        <div class="video-header">
            <h2 class="video-title">Demo Video</h2>
        </div>

            <div class="video-center">
            <iframe width="1000" height="600" src="https://www.youtube.com/embed/U0IpLJOu48Y?si=hmagExCw3C0RjnuG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
            </div>

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
                        
                        <span class="label-text">The framework of JanusVLN. Given an RGB-only video stream and navigation instructions, JanusVLN utilizes a dual-encoder to separately extract visual-semantic and spatial-geometric features. It concurrently caches historical key-values from initial and recent sliding window into a dual implicit memory to facilitate feature reuse and prevent redundant computation. Finally, these two complementary features are fused and fed into LLM to predict the next action.</span>
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

        <iframe width="560" height="315" src="https://www.youtube.com/embed/aJXpWluI1-w?si=350fBzfNH79XocD0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

        <iframe width="560" height="315" src="https://www.youtube.com/embed/jB4CL55pJ3c?si=V4WIUZoqUs-kTj_C" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

        <iframe width="560" height="315" src="https://www.youtube.com/embed/QLuO0ce8Qv0?si=kFpC0EoOxMca4Lq5" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
        
        <iframe width="560" height="315" src="https://www.youtube.com/embed/RPJ_i1YAYek?si=fvHxrbsy7J0Vbk2z" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

        <iframe width="560" height="315" src="https://www.youtube.com/embed/7UuqnfXKQbE?si=WmEulBJUe3BA8yc7" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

        <iframe width="560" height="315" src="https://www.youtube.com/embed/R4fwQuK5t-s?si=xuXGoZ4FRzvWHZHt" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
        
        
    </div>
</div>



<div class="technical-overview-section" id="overview">
    <div class="overview-container">
        <div class="overview-header">
            <h2 class="overview-title">VLN-CE Visualization</h2>
        </div>

        <iframe width="560" height="315" src="https://www.youtube.com/embed/Gt48PnnfNdc?si=t8594wB2u3Laz2Di" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

        <iframe width="560" height="315" src="https://www.youtube.com/embed/Ac7jSX2ryPg?si=-IWl65Q2VnX--R0P" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
        

        <iframe width="560" height="315" src="https://www.youtube.com/embed/s3lv3pr9ObY?si=RhLzYbPAiNOugU2H" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

        <iframe width="560" height="315" src="https://www.youtube.com/embed/0tBRSu-5-SA?si=AOZXPXBB7137bVPK" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

        <iframe width="560" height="315" src="https://www.youtube.com/embed/Fun5oPmZqZs?si=xcKxhZgM9oALE5eL" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

        <iframe width="560" height="315" src="https://www.youtube.com/embed/KqBtCfiAcGc?si=rHk0TgmNSRFa0W1W" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

        
        
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
                @article{zeng2025janusvln,
                title={JanusVLN: Decoupling Semantics and Spatiality with Dual Implicit Memory for Vision-Language Navigation},
                author={Zeng, Shuang and Qi, Dekang and Chang, Xinyuan and Xiong, Feng and Xie, Shichao and Wu, Xiaolong and Liang, Shiyi and Xu, Mu and Wei, Xing},
                journal={arXiv preprint arXiv:2509.22548},
                year={2025}
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




