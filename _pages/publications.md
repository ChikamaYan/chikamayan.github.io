<!-- ---
layout: page
permalink: /publications/
title: publications
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>

<b>Gaussian Head & Shoulders: High Fidelity Neural Upper Body Avatars with Anchor Gaussian Guided Texture Warping</b>
<br>
<b>Tianhao Wu</b>, Jing Yang, Zhilin Guo, Jingyi Wan, Fangcheng Zhong, Cengiz Oztireli
<br>
Arxiv
<br>

<button type="button" onclick="location.href = 'https://gaussian-head-shoulders.netlify.app/';">Project Page</button>
<button type="button" onclick="location.href = 'https://arxiv.org/abs/2405.12069';">Paper</button>

<br>
<br>




<b>αSurf: Implicit Surface Reconstruction for Semi-Transparent and Thin Objects with Decoupled Geometry and Opacity</b>
<br>
<b>Tianhao Wu</b>, Hanxue Liang, Fangcheng Zhong, Gernot Riegler, Shimon Vainer, Cengiz Oztireli
<br>
Arxiv
<br>

<button type="button" onclick="location.href = 'https://alphasurf.netlify.app/';">Project Page</button>
<button type="button" onclick="location.href = 'https://arxiv.org/abs/2303.10083';">Paper</button>

<br>
<br>


<b>D<sup>2</sup>NeRF: Self-Supervised Decoupling of Dynamic and Static Objects from a Monocular Video</b>
<br>
<b>Tianhao Wu</b>, Fangcheng Zhong, Andrea Tagliasacchi, Forrester Cole, Cengiz Oztireli
<br>
NeuRIPS 2022
<br>

<button type="button" onclick="location.href = 'https://d2nerf.github.io/';">Project Page</button>
<button type="button" onclick="location.href = 'https://arxiv.org/abs/2205.15838';">Paper</button>

<br>
<br>


<b>Kubric: a scalable dataset generator</b>
<br>
Klaus Greff and Francois Belletti and Lucas Beyer and Carl Doersch and
Yilun Du and Daniel Duckworth and David J Fleet and Dan Gnanapragasam and
Florian Golemo and Charles Herrmann and Thomas Kipf and Abhijit Kundu and
Dmitry Lagun and Issam Laradji and Hsueh-Ti (Derek) Liu and Henning Meyer and
Yishu Miao and Derek Nowrouzezahrai and Cengiz Oztireli and Etienne Pot and
Noha Radwan and Daniel Rebain and Sara Sabour and Mehdi S. M. Sajjadi and Matan Sela and
Vincent Sitzmann and Austin Stone and Deqing Sun and Suhani Vora and Ziyu Wang and
<b>Tianhao Wu</b> and Kwang Moo Yi and Fangcheng Zhong and Andrea Tagliasacchi
<br>
CVPR 2022
<br>

<button type="button" onclick="location.href = 'https://github.com/google-research/kubric';">Project Page</button>
<button type="button" onclick="location.href = 'https://arxiv.org/abs/2203.03570';">Paper</button>

 -->
