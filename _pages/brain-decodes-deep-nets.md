---
layout: none
title: Brain Decodes Deep Nets
permalink: /brain-decodes-deep-nets
nav: false
subtitle: null
---
<link rel="stylesheet" href="{{ site.baseurl | prepend: site.url }}/custom.css">

<div style="display: flex; flex-direction: column; align-items: center; justify-content: center; height: 100vh; text-align: center;">
  <!-- <div>
    <img src="assets/custom_images/slides_teaser.png" width="100%" style="margin-left:0%; margin-right:0%">
  </div> -->


<iframe width="800" height="450" src="https://www.youtube.com/embed/1ZITyYGNLz0" title="Brain Decodes Deep Nets" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<!-- <div style="margin-top:100px;">
We developed a tool for visualizing and analyzing large pre-trained vision models by mapping them onto the brain, thus exposing their hidden inside. 
</div>
<div>
Highlights: We found remarkable differences for same architecture models trained with different objectives, and same objective but larger model sizes.
</div> -->

<div style="margin-top:30px;">
<h2> <em> The brain is massive; Deep networks are massive. </em> </h2>
<!-- <h3> <em> What can these two massive systems, tell about each other? </em> </h3> -->
<h2> <a style="color:#09AD94;"> <em> <span id="typing-text2"></span> </em>|</a></h2>
</div>

  <h1 style="margin-top: 60px;">Brain Decodes Deep Nets</h1>
  <div style="margin-top: 0px;">Huzheng Yang &emsp; James Gee* &emsp; Jianbo Shi*</div>
  <div> University of Pennsylvania </div>
  <div style="font-size: small"> *: co-advise </div>

  <div style="margin-top: 40px; font-size: large">
    <p style="display: inline-block;">
      <a href="https://arxiv.org/abs/2312.01280" style="text-decoration: underline; color: lightblue; margin-right: 10px;">paper</a>
      <a href="https://github.com/huzeyann/BrainDecodesDeepNets" style="text-decoration: underline; color: lightblue; margin-right: 10px;">code</a>
      <!-- <a href="https://www.youtube.com/TODO" style="text-decoration: underline; color: lightblue; margin-right: 10px;">video</a> -->
      <!-- <a href="https://penno365-my.sharepoint.com/:p:/g/personal/huze_upenn_edu/EcuvlCSxjSBDk719Q_Dxc7ABNUebclx8wIUKAg2VGKwNXQ?e=a0oMma" style="text-decoration: underline; color: lightblue; margin-right: 10px;">slides</a> -->
      <!-- <a href="https://twitter.com/HuzeYann/TODO" style="text-decoration: underline; color: lightblue;">discussion</a> -->
    </p>
  </div>
</div>

<script src="https://cdn.jsdelivr.net/npm/typed.js@2.0.11"></script>
<script src="{{ site.baseurl | prepend: site.url }}/typing2.js"></script>




**TL;DR**: We visualize pre-trained vision models by mapping them onto the brain, thus exposing their hidden inside. Visualization is a by-product of brain encoding model: predict brain fMRI measurements in response to images.

{% include figure.html path="assets/custom_images/bddn_fig1.png" class="img-fluid rounded z-depth-1" %}

### Methods
**Brain encoding model** over-simplified: 
1. *input* image, extract features from pre-trained deep nets
2. *feature selection* for each brain voxel (FactorTopy)
3. linear transformation on selected feature, *output* each brain voxel

The intuitive understanding for our visualization is: each brain voxel asks the question, "which network **layer/space/scale/channel** best predicts my brain response?". 

<img width="800" align="middle" src="assets/custom_images/learning.gif" border="0"> 

### Results
Our analysis and visualization shows:
1. Inner layer layouts of supervised and un-supervised models are different.
2. Larger model have less efficient inner layer layout.
3. Fine-tuning on small datasets change the layer layouts.


{% include figure.html path="assets/custom_images/layer_selectors.png" class="img-fluid rounded z-depth-1" %}

{% include figure.html path="assets/custom_images/channel_big.png" class="img-fluid rounded z-depth-1" %}
