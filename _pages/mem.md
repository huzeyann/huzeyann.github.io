---
layout: home
title: Mem
permalink: /mem
nav: false
subtitle: null
---
<link rel="stylesheet" href="{{ site.baseurl | prepend: site.url }}/custom.css">

<div>
<img src="assets/custom_images/memory.png" width="80%" style="margin-left:10%; margin-right:10%">
</div>

<div id="container-header">

<div style="text-align: center;"><p><h3>Brain is able to...</h3></p></div>
<div style="margin-top: -15px; text-align: center;"><p><h3><span id="typing-text"></span></h3></p></div>
</div>




<script src="https://cdn.jsdelivr.net/npm/typed.js@2.0.11"></script>
<!-- <script src="{{ site.baseurl | prepend: site.url }}/typing.js">] -->


<script>
window.onload = function() {
  new Typed('#typing-text', {
    strings: ["distinguish novel and old images", "think about an image without looking at it", "look at an image without thinking about it"],
    typeSpeed: 50,
    // startDelay: 100,
    backDelay: 2000,
    fadeOut: false,
    backSpeed: 40,
    smartBackspace: true,
    loop: true,
    showCursor: false
  });
};
</script>