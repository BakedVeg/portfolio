---
title: "HEM's Last Visitor: Flower Animation"
date: 2023-07-25T15:34:30-04:00
categories:
  - blog
tags:
  - Houdini
  - Substance
---

The goal of this project was to extend my understanding of vertex-animated textures, focusing on how best to split and texture the resulting geometry. The initial unfolding of the flower is essentially a setup I found from Ian Frederick (link at the bottom). It's a fairly simple vellum cloth sim that gets reversed at the end, as you'll see. The pod it blooms from is a separate sim that uses the initial flower blooming as a collider. In this breakdown, I'll walk you through the Houdini networks, showing the important parameter changes, as well as the textures that were made in Substance Designer.

<div style="clear: both;">
    <h2></h2>
    <p></p>
</div>
<br>

<img src="https://bakedveg.github.io/portfolio/assets/gif/BloomingFlower.gif">

<br>
<br>

<div style="clear: both;">
    <h2>Petal Creation</h2>
    <p>Text</p>
</div>

<img src="https://bakedveg.github.io/portfolio/assets/gif/LeafCreationandUVs.png">

<br>

<img src="https://bakedveg.github.io/portfolio/assets/gif/GroupStartEndandRemesh.png">

<br>

<img src="https://bakedveg.github.io/portfolio/assets/gif/BendPetal.png">

<br>



<div style="clear: both;">
    <h2>Positioning and Animating</h2>
    <p>Text</p>
</div>

<img src="https://bakedveg.github.io/portfolio/assets/gif/BendPetal.png">


<div style="clear: both;">
    <h2></h2>
    <p>If you have any questions or comments don't hesitate to reach out. My contact information is linked on the left and at the bottom. Til next time!</p>
</div>

Ian Frederick's setup here: https://www.youtube.com/watch?v=WQSdMX-z7U4&t=26s

<div style="clear: both;">
    <h2></h2>
    <p></p>
</div>



<br>



<div style="clear: both;">
    <h2>Full Network</h2>
    <p></p>
</div>
<img src="https://bakedveg.github.io/portfolio/assets/images/InsertImage.png">
