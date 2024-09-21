---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
- **Hao-Fang Cheng** , Yi-Ching Ho, and Cheng-Wei Chen. "DentiBot: System Design and 6-DoF Hybrid Position/Force Control for Robot-Assisted Endodontic Treatment." *arXiv preprint arXiv:2310.09691* (2023). (Submitted to *Transactions on Robotics*) [Link](https://arxiv.org/pdf/2310.09691) 
- **Hao-Fang Cheng** , Yi-Chan Li, Yi-Ching Ho and Cheng-Wei Chen. "Force-guided alignment and file feedrate control for robot-assisted endodontic treatment." *2022 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)*. IEEE, 2022. [Link](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9981393) 
- Chun-Yeon Lin, Hao-Tse Chen, **Hao-Fang Cheng** , and Yu-Jun He. "Electrical Impedance Sensing System Design for Abnormal Object Detection." *2021 IEEE/ASME International Conference on Advanced Intelligent Mechatronics (AIM)*. IEEE, 2021. (Best Paper Finalist) [Link](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9517604)

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
