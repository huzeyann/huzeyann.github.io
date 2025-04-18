---
layout: none
title: Brain Decodes Deep Nets
permalink: /brain-decodes-deep-nets
nav: false
subtitle: null
---
<link rel="stylesheet" href="{{ site.baseurl | prepend: site.url }}/custom.css">

<!-- <div style="display: flex; flex-direction: column; align-items: center; justify-content: center; height: 100vh; text-align: center;"> -->
<div style="display: flex; flex-direction: column; align-items: center; justify-content: center; text-align: center;">
  <!-- <div>
    <img src="assets/custom_images/slides_teaser.png" width="100%" style="margin-left:0%; margin-right:0%">
  </div> -->
<!-- <div style="margin-top:30px;">
<iframe width="800" height="450" src="https://www.youtube.com/embed/aKGO7Qd93_w?rel=0?version=3&autoplay=1&controls=0&&showinfo=0&loop=1​" title="[2min paper] Brain Decodes Deep Nets" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div> -->

<div style="margin-top:30px;">
<video width="800" height="450" controls muted autoplay loop>
  <source src="assets/videos/brain_decodes_deep_nets_2min.mp4" type="video/mp4">
  Your browser does not support the video tag.
  <iframe width="800" height="450" src="https://www.youtube.com/embed/aKGO7Qd93_w?rel=0?version=3&autoplay=1&controls=0&&showinfo=0&loop=1​" title="[2min paper] Brain Decodes Deep Nets" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</video>
</div>


<!-- <div style="margin-top:100px;">
We developed a tool for visualizing and analyzing large pre-trained vision models by mapping them onto the brain, thus exposing their hidden inside. 
</div>
<div>
Highlights: We found remarkable differences for same architecture models trained with different objectives, and same objective but larger model sizes.
</div> -->

<div style="margin-top:30px;">
<h2> <em> Brain is massive; Deep nets are massive. </em> </h2>
<!-- <h3> <em> What can these two massive systems, tell about each other? </em> </h3> -->
<h2> <a style="color:#09AD94;"> <em> <span id="typing-text2"></span> </em>|</a></h2>
</div>

  <h1 style="margin-top: 60px;">Brain Decodes Deep Nets</h1>
  <div style="margin-top: 0px;">Huzheng Yang &emsp; James Gee* &emsp; Jianbo Shi*</div>
  <div> University of Pennsylvania </div>
  <div style="font-size: small"> *: co-advise </div>

  <div style="margin-top: 40px; font-size: large">
    <p style="display: inline-block;">
      <a> CVPR'24 </a>
      <a href="https://arxiv.org/abs/2312.01280" style="text-decoration: underline; color: lightblue; margin-right: 10px;">paper</a>
      <a href="https://github.com/huzeyann/BrainDecodesDeepNets" style="text-decoration: underline; color: lightblue; margin-right: 10px;">code</a>
      <a href="https://twitter.com/HuzeYann/status/1731921097203790141?s=20" style="text-decoration: underline; color: lightblue;">twitter</a>
      <!-- <a href="https://youtu.be/bLgcfVN3hU4" style="text-decoration: underline; color: lightblue; margin-right: 10px;">talk online</a> -->
      <!-- <a href="https://penno365-my.sharepoint.com/:p:/g/personal/huze_upenn_edu/EcuvlCSxjSBDk719Q_Dxc7ABNUebclx8wIUKAg2VGKwNXQ?e=a0oMma" style="text-decoration: underline; color: lightblue; margin-right: 10px;">slides</a> -->
      <!-- <a href="https://twitter.com/HuzeYann/TODO" style="text-decoration: underline; color: lightblue;">discussion</a> -->
    </p>
  </div>

  

  <!-- <div style="margin-top:50px;">

  <h3> TL;DR </h3>
  <div> We visualize pre-trained vision models by mapping them onto the brain, thus exposing their hidden inside. Visualization is a by-product of brain encoding model: predict brain fMRI measurements in response to images. </div>

  <div><img width="800" align="middle" src="assets/custom_images/bddn_fig1.png" border="0"></div>
  <div>The intuitive understanding for our visualization is: each brain voxel do feature selection, "which network **layer/space/scale/channel** best predicts my brain response?".</div>


  <h3> Methods </h3>
  <h4>Brain encoding model over-simplified:</h4>
  <div>1. <em>input</em> image, extract features from pre-trained deep nets</div>
  <div>2. <em>feature selection</em> for each brain voxel (FactorTopy)</div>
  <div>3. divnear transformation on selected feature, <em>output</em> each brain voxel</div> 

  <!-- <div><img width="800" align="middle" src="assets/custom_images/learning.gif" border="0"></div>
  <div>The intuitive understanding for our visualization is: each brain voxel asks the question, "which network **layer/space/scale/channel** best predicts my brain response?".</div> -->

  <!-- <h3> Findings </h3>
  <h4>same ViT architecture for all models</h4>
  <div>1. Inner layer layouts of supervised and un-supervised models are different</div>
  <div>2. Larger model have less efficient inner layer layout (expect for CLIP)</div>
  <div>3. Fine-tuning on small datasets change the layer layouts</div>
  
  <div><img width="800" align="middle" src="assets/custom_images/layer_selectors.png" border="0"></div>

  <div><img width="800" align="middle" src="assets/custom_images/channel_big.png" border="0"></div>

  
  </div> --> 

</div>

<script src="https://cdn.jsdelivr.net/npm/typed.js@2.0.11"></script>
<script src="{{ site.baseurl | prepend: site.url }}/typing2.js"></script>


<br/><br/><br/><br/><br/>

<div style="margin-top:30px;">
<iframe width="800" height="450" src="https://www.youtube.com/embed/Qh49zQQCW1g" title="[CVPR 2024] Brain Decodes Deep Nets" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

## Main Story 

## *visualize pre-trained vision models by mapping model onto the brain*.

<br/><br/>

### Neuroscience Background

Visual brain is organized into regions, each region has specialized functions.
For example, V1 does edge-detection and orientation filtering. FFA is face selective, if there’s a face, neurons in FFA fire.

In the brain, Image processing and feature computation are organized in a hierarchical and largely feed-forward fashion. V1 is the initial visual region that physically connected to input from the eyes. Representation in the brain become increasingly abstract from V1 onwards to other regions.


<!-- <div><img width="800" align="middle" src="assets/custom_images/neuroscience_background.png" border="0"></div> -->
<div><img width="800" align="middle" src="assets/gif/brain_background.gif" border="0"></div>



Visualization (*Brain-to-Network Alignment*) is a by-product of brain encoding model, each brain voxel selects:

1. "which <strong>layer</strong> best predicts my brain response?"
2. "which <strong>space</strong> best predicts my brain response?"
3. "which <strong>scale</strong> best predicts my brain response?"
4. "which <strong>channel</strong> best predicts my brain response?"

<div><img width="800" align="middle" src="assets/custom_images/bddn_fig1_v2.png" border="0"></div>
> The intuitive understanding for our visualization is: each brain voxel asks the question, "which network *layer/space/scale/channel* best predicts my brain response?". 


### Methods
*Brain encoding model* over-simplified: 
1. *input* image, extract features from pre-trained deep nets
2. *feature selection* for each brain voxel
3. linear regression on selected features, *output* each brain voxel

<div><img width="800" align="middle" src="assets/custom_images/learning.gif" border="0"></div>

### Results
<!-- Brian-to-Network alignment shows:
1. There's huge difference in intermediate layers of models trained with same architecture but different objective and data.
2. Larger model have less brain-like layer layout.
3. Fine-tuning on small datasets change existing brain-to-network alignment. -->



<div><img width="800" align="middle" src="assets/custom_images/layer_selectors.png" border="0"></div>

<div><img width="800" align="middle" src="assets/custom_images/channel_big.png" border="0"></div>

<!-- ### Takeaway
Brain-to-Network alignment could be a way to find modular and generalizable model, we found CLIP has the best brain-net alignment: 
1. Align with brain's hierarchical layout.
2. Better brain-net alignment when scaled up size and data.
3. Least catastrophic forgetting in finetuning. -->
