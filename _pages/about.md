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

I am a Ph.D. student in the [Department of Computer Science](https://www.cs.umd.edu/) at the [University of Maryland, College Park](https://www.umd.edu/), advised by [**Prof. Heng Huang**](https://www.cs.umd.edu/~heng/).

Before joining UMD, I received my M.S. degree from Shanghai Jiao Tong University, where I was advised by [**Prof. Xiaolin Huang**](http://www.pami.sjtu.edu.cn/en/xiaolin). I received my B.E. degree in Automation from Xi'an Jiaotong University.

My research interests include **machine learning, LLM agents, AI safety, and efficient LLM systems**, with a focus on building safer and more efficient AI systems. I am always open to academic discussions and collaborations; please feel free to reach out via email.


# 🔥 News

<div id="news-items" markdown="1">

- **2026.08:** I started my Ph.D. study in Computer Science at the **University of Maryland, College Park**.

- **2026.07:** 🎉 Our paper “[**InjecMEM: Memory Injection Attack on LLM Agent Memory Systems**](https://arxiv.org/abs/2503.18126)” was accepted to **COLM 2026**!

- **2026.06:** 🎉 Our paper “[**Stochastic Optimal Control Sampling for Diffusion Inverse Problems**](https://arxiv.org/abs/2606.28785)” was accepted to **ECCV 2026**!

- **2026.01:** 🎉 Our paper “[**RAIN-Merging: A Gradient-Free Method to Enhance Instruction Following in Large Reasoning Models with Preserved Thinking Format**](https://openreview.net/forum?id=PO2iULmu5e)” was accepted to **ICLR 2026** as an **Oral presentation**!

- **2025.05:** 🎉 Our paper “[**Primphormer: Efficient Graph Transformers with Primal Representations**](https://openreview.net/forum?id=fMAihjfJij)” was accepted to **ICML 2025**!

- **2025.01:** 🎉 My first first-author paper, “[**Simulating Training Dynamics to Reconstruct Training Data from Deep Neural Networks**](https://openreview.net/forum?id=ZJftXKy12x),” was accepted to **ICLR 2025**!

</div>

<div style="text-align: center; margin-top: 2px; margin-bottom: 8px;">
  <button
    id="news-toggle"
    type="button"
    onclick="toggleNews()"
    style="
      display: none;
      border: none;
      background: none;
      color: #2a5db0;
      cursor: pointer;
      font-size: 0.95em;
      padding: 3px 12px;
    ">
    More ▾
  </button>
</div>

<style>
  #news-items:not(.expanded) ul > li:nth-child(n+6) {
    display: none;
  }

  #news-toggle:hover {
    text-decoration: underline;
  }
</style>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const newsItems = document.querySelectorAll("#news-items ul > li");
  const button = document.getElementById("news-toggle");

  if (newsItems.length > 5) {
    button.style.display = "inline-block";
  }
});

function toggleNews() {
  const news = document.getElementById("news-items");
  const button = document.getElementById("news-toggle");

  news.classList.toggle("expanded");

  if (news.classList.contains("expanded")) {
    button.innerHTML = "Less ▴";
  } else {
    button.innerHTML = "More ▾";
  }
}
</script>


# 📝 Selected Publications

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">COLM 2026</div><img src='images/injecmem.png' alt="InjecMEM" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

### [InjecMEM: Memory Injection Attack on LLM Agent Memory Systems](https://arxiv.org/abs/2608.23471)

**Hanling Tian**, Gengyu Zhang, Zeyang Sha, Jingying Wang, Yuhang Liu, Zhehao Huang, Kun Yang, Xiaolin Huang

**Conference on Language Modeling (COLM), 2026**

[**OpenReview**](https://openreview.net/forum?id=VbXN1Ny912) &nbsp; [**arXiv**](https://arxiv.org/abs/2608.23471) &nbsp; [**Code**](https://github.com/BlueBlood6/InjecMEM)

We introduce **InjecMEM**, a memory injection attack against LLM agents with persistent memory. A single malicious interaction can poison the memory system and influence the agent's responses to future benign queries.

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICLR 2025</div><img src='images/simudy.png' alt="SimuDy" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

### [Simulating Training Dynamics to Reconstruct Training Data from Deep Neural Networks](https://openreview.net/forum?id=ZJftXKy12x)

**Hanling Tian**, Yuhang Liu, Mingzhen He, Zhengbao He, Zhehao Huang, Ruikai Yang, Xiaolin Huang

**International Conference on Learning Representations (ICLR), 2025**

[**OpenReview**](https://openreview.net/forum?id=ZJftXKy12x) &nbsp; [**Code**](https://github.com/BlueBlood6/SimuDy) &nbsp; [**Slides**](https://iclr.cc/media/iclr-2025/Slides/29225.pdf) &nbsp; [**Poster**](https://iclr.cc/media/PosterPDFs/ICLR%202025/29225.png?t=1744123306.3932734)

We propose **SimuDy**, which reconstructs training data from trained deep neural networks by explicitly simulating the training dynamics from model initialization to the final trained parameters.

</div>
</div>


# 📚 Other Publications

- **[Stochastic Optimal Control Sampling for Diffusion Inverse Problems](https://arxiv.org/abs/2606.28785)**  
  Jie Zhang, Youmei Qiu, **Hanling Tian**, Jingyuan Zhang, Xiang Yin, Xiaolin Huang.  
  **European Conference on Computer Vision (ECCV), 2026.**  

- **[RAIN-Merging: A Gradient-Free Method to Enhance Instruction Following in Large Reasoning Models with Preserved Thinking Format](https://openreview.net/forum?id=PO2iULmu5e)**  
  Zhehao Huang, Yuhang Liu, Baijiong Lin, Yixin Lou, Zhengbao He, **Hanling Tian**, Tao Li, Xiaolin Huang.  
  **International Conference on Learning Representations (ICLR), 2026. Oral.**  

- **[Primphormer: Efficient Graph Transformers with Primal Representations](https://openreview.net/forum?id=fMAihjfJij)**  
  Mingzhen He, Ruikai Yang, **Hanling Tian**, Youmei Qiu, Xiaolin Huang.  
  **International Conference on Machine Learning (ICML), 2025.**  


# 📖 Education

- **2026 – Present**, Ph.D. in Computer Science, **University of Maryland, College Park**  
  Advisor: [Prof. Heng Huang](https://www.cs.umd.edu/~heng/)

- **2023 – 2026**, M.S., **Shanghai Jiao Tong University**  
  Institute of Image Processing and Pattern Recognition  
  Advisor: [Prof. Xiaolin Huang](http://www.pami.sjtu.edu.cn/en/xiaolin)

- **2019 – 2023**, B.E. in Automation, **Xi'an Jiaotong University**


# 💻 Experience

- **Microsoft Research Asia (MSRA)** — Research Intern, DKI Group  
  Research on multimodal learning, layout understanding, and generative models.

- **Ant Group** — Research Intern, AI Safety  
  Research on the safety and security of LLM agents and memory systems.


# 📝 Academic Service

- **Reviewer:** ICML 2026, COLM 2026, NeurIPS 2026, MICCAI 2026 Workshop AMPLIFAI
- **Program Committee:** AAAI 2027


# 🌎 Visitors

<div style="width: 520px; max-width: 100%; margin: 15px auto 20px auto; text-align: center;">

<script type="text/javascript" id="mapmyvisitors" src="//mapmyvisitors.com/map.js?d=zTSIX_4sfuATLpOY7hbj8tBeMnIHrcF7uxWx1-zhNDQ&cl=ffffff&w=a"></script>

</div>
