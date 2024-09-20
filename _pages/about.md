---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
<p align = "justify"> 
I am a research assistant at National Taiwan University, where my research focuses on robot kinematics, sensor fusion, and control. I am fortunate to be advised by 
  <a href="https://cwchenee.wixsite.com/nasa-ntuee">Prof. Cheng-Wei Chen</a> from the Department of Electrical Engineering at National Taiwan University, working on robot-assisted endodontic treatment. Additionally, I had the opportunity to be mentored by <a href="https://mistlab.ca/">Prof. Giovanni Beltrame</a> from the Department of Computer Science at Polytechnique Montreal during a six-month research internship, where I integrated UWB systems with multi-drone and multi-vehicle networks.
</p>
# Research Project

## DentiBot: First robot designed for endodontic treatment
Keywords: Robot autonomy, sensor module design, hybrid control 
<p align = "justify"> 
<iframe width="560" height="315" src="https://www.youtube.com/embed/n4k5wcZihyk?si=lVZqIsB7bOsqPL4D" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
  
In this project, I intergrated the DentiBot, the first robot specifically designed for dental endodontic treatment. The DentiBot is equipped with a force and torque sensor, as well as a string-based Patient Tracking Module, allowing for real-time monitoring of endodontic file contact and patient movement. We propose a 6-DoF hybrid position/force controller that enables autonomous adjustment of the surgical path and compensation for patient movement, while also providing protection against endodontic file fracture. In addition, a file flexibility model is incorporated to compensate for file bending. Pre-clinical evaluations performed on acrylic root canal models and resin teeth confirm the feasibility of the DentiBot in assisting endodontic treatment. This work has been published to IROS 2022 and submitted to Transaction on Robotics (T-RO). 
Relative Publishment:
</p>
<img src="images/dentibot.png">
<details>
<summary>Read More</summary>
<p align = "justify">
 The DentiBot utilizes 6-DoF patient tracking module, which employs a string-based parallel kinematic mechanism as a passive pose measurement device. This mechanism determines the relative pose between two rigid bodies by measuring the lengths of six strings that connect them. The strings are securely attached to a custom-made dental anchor, allowing the PTM to fixate onto the teeth while providing sufficient workspace for the dental handpiece. The anchor points for the strings are strategically distributed to minimize the risk of string crossing and avoid kinematic singularities. A Newton-Raphson method is applied to calculate the relative pose. Notebly, the PTM has demonstrated a precision of <strong>1 mm</strong> and <strong>1 degree</strong>.
</p>
<img src="images/dentibot_ptm.png">

<p align = "justify">
The distinctive feature of endodontic files is their flexibility. However, this flexibility introduces additional displacement when external forces are applied, requiring careful compensation. In this study, I account for file flexibility by incorporating the file deflection as a position offset. A tapered beam model is used to estimate the file's bending. Additionally, the file's characteristic parameters are determined experimentally to ensure that the model's estimated deflection aligns with the experimental data, as shown in Figure c. 
</p>
<img src="images/dentibot_file_model.png">

<p align = "justify"> 
The block diagram below shows the proposed 6-DoF hybrid position/force control. In the inner-loop position control (yellow box), the robotic manipulator receives velocity commands <span>p&#x0307;<sub>cmd</sub></span> and adjusts its pose relative to the patient to reach the desired value <span>p<sub>d</sub></span>. Here, <span>&#x0394;p</span> denotes the patient movement, and <span>p<sub>s</sub></span> represents the relative pose measured from the PTM. In the outer-loop force control (green box), the contact force <span>&#x1D701;<sub>s</sub></span> between the endodontic file and root canal, measured by the force/torque sensor, is sent to the file flexibility compensator and admittance controller. These components generate the pose adjustments <span>p<sub>f</sub></span> and <span>p<sub>adm</sub></span> to help the DentiBot achieve the desired contact force <span>&#x1D701;<sub>d</sub></span>.
</p>

<img src="images/Hybrid-control-diagram.png">
</details>

## Human-Drone Interaction by using UWB Localization system 
![human_drone](images/human-drone-interaction.png)
<p align = "justify"> 
In this project, I deployed six Cogniflies <a href="https://thecognifly.github.io/">Cogniflies </a>, collision Resilient UAVs, in an exhibition hall to interact with dancers. An Ultra-Wideband (UWB) system was used to localize both the drones and the tags carried by humans, with the advantage of UWB being its ability to penetrate obstacles. I fine-tuned the Extended Kalman Filter (EKF) within the estimator to enhance localization accuracy. Additionally, I integrated the <a href="https://ieeexplore.ieee.org/abstract/document/7759558">Buzz controller </a> from another project into this work, enabling users to control the drones—such as taking off, swarming, and landing—by moving the tag in their hands.
</p>

## Enhancing Swarm-SLAM by adding UWB distance constrain 
![Swarm Slam](images/swarm slam.png)
<p align = "justify"> 
Collaborative Simultaneous Localization and Mapping (C-SLAM) is essential for successful multirobot operations in complex environments. Our lab has already developed <a href="https://github.com/MISTLab/Swarm-SLAM">Swarm-SLAM</a> for multi-vehicle SLAM. However, merging maps from different robots remains a challenging task, demanding significant computational resources. In this work, I equipped each robot with Ultra-Wideband (UWB) sensors, allowing them to obtain relative distance measurements without line of sight. By integrating this relative distance into the pose graph as an additional constraint, the optimization algorithm for localization is improved, enabling the robots to merge their maps more efficiently and in a shorter time.
</p>

## Electrical Impedance Sensing System Design for Abnormal Object Detection
![EIT](images/EIT.png)
<p align = "justify"> 
This project proposed a design for an electrical impedance (EI) sensing system. For the part of physical modeling, the harmonic electric fields of the EI sensing system are formulated by the distributed parameter element (DPE) method to calculate the electrode potentials for several injection patterns of different abnormal object distributions, and the computed electrode potentials are feed into a deep neural network (DNN) to estimate the location and size of the abnormal object. For the part of system development, an electric circuit that integrates the multiplexer and Howland pump is utilized to switch the current injection electrodes and control the injection currents. The harmonic electric fields computed by the DPE method are verified by the FEA software, and the effects of utilizing the DNN for abnormal object detection are numerically validated. The proposed design, along with a prototype of the EI sensing system, which is conducted on two kinds of materials, phantom and biological objects, have been experimentally compared. 
</p>
![EIT](images/EIT_DNN.png)

# Competition or Course Project

## TDK National Creative Design Competition: Using UAV for autonomous driving, throwing, and landing
<p align = "justify"> 
<iframe width="560" height="315" src="https://www.youtube.com/embed/48ojjCHAxoY?si=_p-hFNK9tuSgmWfO" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
In October 2019, I participated in the 2020 TDK National Creative Design Competition as part of a university team, where we achieved 2nd place in the Flying Group category. I led the first team from our university to compete in this event, where we designed and built an autonomous drone from scratch. The drone was capable of following a designated ground trajectory, navigating obstacles, and delivering payloads.
  
As the team leader, I was responsible for organizing the team, delegating tasks, and ensuring resource availability. My leadership and technical efforts were instrumental in guiding the team to a successful outcome, resulting in a fully functional and competitive drone design.
</p>
## Robotics Final Project: Using Manipualtor to Solve Puzzle 
<iframe width="560" height="315" src="https://www.youtube.com/embed/C8wDrQi4jkE?si=UH1HqMph3G2K6uZH" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Mechatronics Final Project: Velocity Control for Panuatic Automobile
<iframe width="560" height="315" src="https://www.youtube.com/embed/jzHP1wdxl_o?si=roOJDU1zsC2ZX86_" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


