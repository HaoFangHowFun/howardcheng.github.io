---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
- **H.-F. Cheng** , Y.-C. Ho, and C. -W. Chen, "Autonomous Dental Surgery for Root Canal Treatment: Compensating for Robot-Patient Misalignment and File Deflection.", IEEE Transactions on Automation Science and Engineering (T-ASE), 2025. doi: 10.1109/TASE.2025.3611997 [Link](https://ieeexplore.ieee.org/document/11174012) 
- **H.-F. Cheng** , Y. -C. Li, Y. -C. Ho and C. -W. Chen, "Force-Guided Alignment and File Feedrate Control for Robot-Assisted Endodontic Treatment," 2022 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), Kyoto, Japan, 2022, pp. 1841-1847, doi: 10.1109/IROS47612.2022.9981393. [Link](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9981393) 
- C. -Y. Lin, H. -T. Chen, **H. -F. Cheng**, and Y. -J. He, "Electrical Impedance Sensing System Design for Abnormal Object Detection," 2021 IEEE/ASME International Conference on Advanced Intelligent Mechatronics (AIM), Delft, Netherlands, 2021, pp. 1313-1318, doi: 10.1109/AIM46487.2021.9517604. (Best Paper Finalist) [Link](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9517604)
- C. -W. Chen, Y. -C. Li, and **H. -F. Cheng**. "Endodontic robotic surgical system and endodontic robotic surgical assembly," U.S. Patent No 12,029,509, 2024.


{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
