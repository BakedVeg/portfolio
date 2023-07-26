---
title: "Hammerfish Animation"
date: 2023-07-25T15:34:30-04:00
categories:
  - blog
tags:
  - Houdini
  - 
---

This is a part of some early testing I've been doing for creature animations, meant for a small game that's been knocking around in my head. The idea is to have several animals roaming about the environment. I'm just one person so I felt like my best shot at accomplishing that would be to do all the modeling inside Houdini, rely on CHOPs-driven animation, and a bit of simulation sprinkled throughout to quickly give life to each of the creatures. After modeling and animating, I export them using the VAT output SideFX ships, allowing for much more fauna than what would be possible with bone-based animations. In my mind, the modeling/animation has to be procedural so that I can create the animations as I model each piece and add more detail to the animals without having to reanimate pieces I've created before. This serves as a brief walkthrough of the setup for this "Hammerfish". At the bottom of the page, you'll find an image of the full network.


<img src="https://bakedveg.github.io/portfolio/assets/gif/HammerfishAnimLoopAlpha.gif">




<div style="clear: both;">
  <div style="float: left; margin-left 1em;">
    <img src="https://bakedveg.github.io/portfolio/assets/gif/HammerfishAnimTopAlpha.gif">
  </div>
  <div>
    <h2>Main Body Creation</h2>
    <p>I started with a sphere, grouped both ends and used soft transforms to get the desired bell shape. Then smoothed the result.</p>
  </div>
</div>

<img src="https://bakedveg.github.io/portfolio/assets/gif/BodyCreationWalkthroughAlpha.gif">


<img src="https://bakedveg.github.io/portfolio/assets/gif/HammerCreationWalkthroughAlpha.gif">

<img src="https://bakedveg.github.io/portfolio/assets/gif/CombinationWalkthroughAlpha.gif">


<div style="clear: both;">
  <div style="float: right; margin-right 1em;">
    <img src="https://bakedveg.github.io/portfolio/assets/gif/VellumTentacleWalkthroughAlpha.gif">
  </div>
  <div>
    <h2>Some title text</h2>
    <p>Some more text that will appear to the left of the image.</p>
  </div>
</div>


<img src="https://bakedveg.github.io/portfolio/assets/images/FinalAssembly.png">

<img src="https://bakedveg.github.io/portfolio/assets/images/FinalTextured.png">

<img src="https://bakedveg.github.io/portfolio/assets/images/HoudiniHammerfishGeoNetwork.png">
