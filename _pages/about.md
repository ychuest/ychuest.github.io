---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>


# 😀 Hi there! 

Welcome to Cheng Yang(杨城)’s website!

Previously I obtained my master degree in computer science from Hunan University of Science and Technology where I was advised by [Prof.Li Peng](https://faculty.hnust.edu.cn/pubtphp/jsjkxygcxy/1050047/chinese/).

I’m currently conducting some research in deep learning, including:    
🌲 **Large Language Models in Bioinformatics**.  
🌱 **Interaction Event Prediction in Bioinformatics**.  
🌿 **Graph Neural Networks for Recommender Systems**. 

I have published several papers in Briefings in Bioinformatics (BIB), IEEE/ACM Transactions on Computational Biology and Bioinformatics (TCBB), and IEEE Journal of Biomedical and Health Informatics ([JBHI](https://ieeexplore.ieee.org/author/37089867636)).

**I'm actively seeking a PHD opportunity. If you have any opportunities, please contact me, I would appreciate it. Thanks 😎!**

# 🔥 News
- *2024.07*: &nbsp;🎉🎉 One paper accepted by JBHI'24.
- *2024.07*: &nbsp;🎉🎉 One co-authored paper is under review by [IJBM](https://www.editorialmanager.com/ijbiomac/Default.aspx) journal reviewers.
- *2023.06*: &nbsp;🎉🎉 One paper accepted by JBHI'23.
- *2022.05*: &nbsp;🎉🎉 One paper accepted by BIB'22.
- *2022.09*: &nbsp;🎉🎉 One co-authored paper accepted by TCBB'22!

# 📝 Publications 

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">JBHI'24</div><img src='../images/MRLHGNN.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">
  
[**Drug repositioning via Multi-view Representation Learning with Heterogeneous Graph Neural Network**](https://ieeexplore.ieee.org/abstract/document/9882129) <img src='https://img.shields.io/github/stars/ychuest/MRLHGNN.svg?style=social&label=Star' alt="sym" height="100%">

Li Peng, **Cheng Yang**, Jiahuai Yang, Yuan Tu, Qingchun Yu, Zejun Li, Min Chen, Wei Liang

- A heterogeneous graph neural network focusing on local structure.
- Transformer's feature fusion mechanism.
- Subgraph feature aggregation.

<div style="display: inline">
    <a href="https://ieeexplore.ieee.org/abstract/document/10613361"> <strong>[paper]</strong></a>
    <a href="https://github.com/ychuest/MRLHGNN"> <strong>[code]</strong></a>
    <a href="https://github.com/ychuest/MRLHGNN"> <strong>[Project Page]</strong></a>
    <a class="fakelink" onclick="$(this).siblings('.abstract').slideToggle()" ><strong>[abstract]</strong></a>
    <div class="abstract"  style="overflow: hidden; display: none;">  
        <p> Exploring simple and efficient computational methods for drug repositioning has emerged as a popular and compelling topic in the realm of comprehensive drug development. The crux of this technology lies in identifying potential drug-disease associations, which can effectively mitigate the burdens caused by the exorbitant costs and lengthy periods of conventional drugs development. However, current computational drug repositioning methods face challenges in accurately predicting drug-disease associations. These challenges include only considering drugs and diseases to construct a heterogeneous graph without including other biological nodes associated with the disease or drug for a more comprehensive heterogeneous graph, as well as not fully utilizing the local structure of heterogeneous graphs and rich semantic features. To address these problems, we propose a Multi-view Representation Learning method (MRLHGNN) with Heterogeneous Graph Neural Network for drug repositioning. This method is based on a collection of data from multiple biological entities associated with drugs or diseases. It consists of a view-specific feature aggregation module with meta-paths and auto multi-view fusion encoder. To better utilize local structural and semantic information from specific views in heterogeneous graph, MRLHGNN employs a feature aggregation model with variable-length meta-paths to expand the local receptive field. Additionally, it utilizes a transformerbased semantic aggregation module to aggregate semantic features across different view-specific graphs. Finally, potential drug-disease associations are obtained through a multi-view fusion decoder with an attention mechanism. Cross-validation experiments demonstrate the effectiveness and interpretability of the MRLHGNN in comparison to nine state-of-the-art approaches. Case studies further reveal that MRLHGNN can serve as a powerful tool for drug repositioning. </p>
    </div>
</div>
  
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">JBHI'23</div><img src='../images/GATCL2CD.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">
  
[**Predicting CircRNA-Disease associations via feature convolution learning with heterogeneous graph attention network**](https://ieeexplore.ieee.org/document/10079096) <img src='https://img.shields.io/github/stars/ychuest/GATCL2CD.svg?style=social&label=Star' alt="sym" height="100%">

Li Peng, **Cheng Yang**, Yifan Chen and Wei Liu

- Multi-kernel feature convolutional learning methods.
- Dynamic Attention Mechanism.
- Heterogeneous Graph Feature Representation Learning.

<div style="display: inline">
    <a href="https://ieeexplore.ieee.org/document/10079096"> <strong>[paper]</strong></a>
    <a href="https://github.com/ychuest/GATCL2CD"> <strong>[code]</strong></a>
    <a href="https://github.com/ychuest/GATCL2CD"> <strong>[Project Page]</strong></a>
    <a class="fakelink" onclick="$(this).siblings('.abstract').slideToggle()" ><strong>[abstract]</strong></a>
    <div class="abstract"  style="overflow: hidden; display: none;">  
        <p> Exploring the relationship between circular RNA (circRNA) and disease is beneficial for revealing the mechanisms of disease pathogenesis. However, a blind search for all possible associations between circRNAs and diseases through biological experiments is time-consuming. Although some prediction methods have been proposed, they still have limitations. In this study, a novel computational framework, called GATCL2CD, is proposed to forecast unknown circRNA-disease associations (CDAs). First, we calculate Gaussian interactive profile kernel (GIP) similarity and semantic similarity for diseases, circRNA sequence similarity and function similarity, and GIPs for circRNAs. Then, we combine them to construct a heterogeneous graph. Thereafter, GATCL2CD proposes a feature convolution learning framework, that uses a multi-head dynamic attention mechanism to obtain different aggregated representations of features that correspond to the nodes in the heterogeneous graph. Then, it extracts rich higher-order features from the stacked feature representations of each node by using of a single-layer convolutional neural network with filter kernels of different sizes. Finally, a pairwise element-wise product operation is implemented to capture the interactions of higher-order feature representations, and a multilayer perceptron neural network is introduced as an efficient classifier for inferring potential CDAs. Major experimental results under 5-fold cross-validation (5-fold CV) on three different datasets show that GATCL2CD is superior to five other state-of-the-art methods. Furthermore, case studies demonstrate the suitability of GATCL2CD as a useful tool for identifying potential disease-related circRNAs. </p>
    </div>
</div>
  
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">BIB'22</div><img src='../images/RNMFLP.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**RNMFLP: Predicting circRNA–disease associations based on robust nonnegative matrix factorization and label propagation**](https://academic.oup.com/bib/article/23/5/bbac155/6582881?login=false) <img src='https://img.shields.io/github/stars/biohnuster/RNMFLP.svg?style=social&label=Star' alt="sym" height="100%">

Li Peng, **Cheng Yang**, Li Huang, Xiang Chen, Xiangzheng Fu and Wei Liu

- Robust non-negative matrix factorisation.
- Multiple subspace feature propagation.
- Convex Optimisation Optimal Solution Method.

<div style="display: inline">
    <a href="https://academic.oup.com/bib/article/23/5/bbac155/6582881?login=false"> <strong>[paper]</strong></a>
    <a href="https://github.com/biohnuster/RNMFLP"> <strong>[code]</strong></a>
    <a href="https://github.com/biohnuster/RNMFLP"> <strong>[Project Page]</strong></a>
    <a class="fakelink" onclick="$(this).siblings('.abstract').slideToggle()" ><strong>[abstract]</strong></a>
    <div class="abstract"  style="overflow: hidden; display: none;">  
        <p> Circular RNAs (circRNAs) are a class of structurally stable endogenous noncoding RNA molecules. Increasing studies indicate that circRNAs play vital roles in human diseases. However, validating disease-related circRNAs in vivo is costly and time-consuming. A reliable and effective computational method to identify circRNA–disease associations deserves further studies. In this study, we propose a computational method called RNMFLP that combines robust nonnegative matrix factorization (RNMF) and label propagation algorithm (LP) to predict circRNA–disease associations. First, to reduce the impact of false negative data, the original circRNA–disease adjacency matrix is updated by matrix multiplication using the integrated circRNA similarity and the disease similarity information. Subsequently, the RNMF algorithm is used to obtain the restricted latent space to capture potential circRNA–disease pairs from the association matrix. Finally, the LP algorithm is utilized to predict more accurate circRNA–disease associations from the integrated circRNA similarity network and integrated disease similarity network, respectively. Fivefold cross-validation of four datasets shows that RNMFLP is superior to the state-of-the-art methods. In addition, case studies on lung cancer, hepatocellular carcinoma and colorectal cancer further demonstrate the reliability of our method to discover disease-related circRNAs. </p>
    </div>
</div>
  
</div>
</div>



# 🎖 Honors and Awards
- *2020-2023(M.Eng.)*: Outstanding Graduate(2023), National Scholarships for Postgraduate Students(2022), Scholarship(2021).


# 📖 Educations
- *2020.09 - 2023.06*, M.Eng. in Computer Science, School of Computer Science and Technology, Hunan University of Science and Technology
- *2023.09 - 2024.05*, Algorithmic Engineer in Hunan Geely Auto Parts Co.
- *2024.06 - (now)*, Junior Engineer of Large Language Models in the Information Office of the Teaching and Research Support Center, National University of Defense Technology.


# 💬 Invited Talks
- *2021.12*, I previously gave an oral presentation at the 21st International Conference on Algorithms and Architectures for Parallel Processing (ICA3PP'21, CCF-C).


# 💻 Internships
- *2024.06 - (now)*, Junior Engineer with Large Language Model joins Network Information Centre of National University of Defence Technology (NUDT), Changsha.

<p align="center"> 
  Visitor times<br>
  <img src="https://profile-counter.glitch.me/yangchengyjs.github.io/count.svg" />
</p>


