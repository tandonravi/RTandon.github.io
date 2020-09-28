---
layout: archive
title: "Research Experiences"
permalink: /research/
redirect_from: 
  - /rs/
  - /researches.html
  
author_profile: true
---

{% include base_path %}

Project 1: Prevent Backdoor Attacks using matching network 
==========================================================
* Problem Statement: How to offend a hide and strong attack with changing several labels or hyperparameters with just one shoot
* Solution: The key to solve this kind of attack is to find how, where and what the attack perform, the contribution of my work is the following:
    * Evaluated whether the initial meta-training by benign users do not include correctly-labeled examples of backdoor classes 
    * Investigated the case where backdoor classes are present, with correct labels, also during fine-tuning.
    * Explored the effects of additional supervised fine-tuning with the different hyperparameters
    * Proposed a defense mechanism applied by each benign user: used just a few labels to predict unseen labels when evaluating the federated model
* Results: This kind of defense mechanism can actually totally eliminate the backdoor attack from federated users
  
<div align="center">
<img src="/images/back1.jpg">
<img src="/images/back2.jpg">
</div>
<br/>

Project 2: Neutral ensemble search on off-line quantization 
===========================================================
* Problem Statement: How to search and compress a model without losing accuracy
* Solution: By training a accuracy predictor to directly measure different quantized model and using evolution method to select the highest predicted model, we can finally evaluate and get the best performance model:
    * Pre-trained model preparing for the quantization and collected dataset to train a accuracy predictor
    * Selected three best model quantized parameters by using evolution search and accuracy predictor 
    * Using neutral ensemble search to search the best performance quantization model
* Results: The model can achieve the same accuracy with the original model with just 1.73MB.

* Demos

<div align="center">
<img src="/images/quan1.jpg">
<img src="/images/quan2.jpg">
<img src="/images/quan3.jpg">
</div>
<br/>

Project 3: Robotic Network Routing Optimization using Multi-Armed Bandit 
============================================================================
* Problem Statement: How to search and manage a best path for the robotic network
* Solution: Motivated by the Multi-Armed Bandits problem, we decided to use Thompson Sampling combined with shortest path algorithm and Bellman Ford algorithm:
    * Compared the regrets of Dijkstra’s algorithm with Thompson Sampling , Upper Confidence Bound and Greedy Algorithm;
    * Chose linear combination of arms (edges) each time rather than one edge each time to avoid exponential growth actions
    * Used the optimal algorithm—Thompson Sampling in the distributed robotic network system with Bellman Ford algorithm to search for the shortest route.
    * Calculated the new bound of regrets for the linear combination Thompson Sampling 
* Results: After enough iterations, which depends on the number of arms, the best path can be chosen.

<div align="center">
<img src="/images/ts1.jpg">
<img src="/images/ts2.jpg">

</div>

Project 4: China Robot Competition, Yibin, Sichuan, China
=========================================================

* Problem statement: prepared for the basketball robot competition which scored for the accurate shoot by the basketball robot, the contribution of my work is the following:
   * Designed and refitted electromagnetic launch system of basketball robot to improve shooting efficiency and hit rate: recharged capacitance with increased voltage, discharged the capacitance through inductor to produce magnetic field which could control pontil of the launch system more preciously
   * Remodeled power source system: changed old linear power supply into switching power supply, adjusted output voltage through modifying duty ratios, installed more shield and grounding measures
   * Applied the optimized neural network on image recognition to process color images and depth map, as well as to use the depth map to measure distance
* Results: our group actually got the highest scores and won the first prize


Project 5: Neural Network Optimization Using Complex Value
=========================================================

* Problem statement: replace real value with complex-valued variables in the neutral network to improve the performance, the contribution of my work is the following:
    * Optimized neural network based on Single-Shot Multi-box Detector (SSD) by replacing real variables with complex-valued variables: batch-processed to normalize complex-values and initialized weight function of complex-values by plural convolutions;  
    * Improved image recognition precision to enable sized bounding box at more accurate testing position; 
    * Reduced data loading of each layer by shrinking matrix’s size to simplify complexity of the neutral network;
    * Modified testing procedure of image recognition to reduce testing duration;
* Results: The complex-valued based model achieved thirty percent higher accuracy than the real-value model
