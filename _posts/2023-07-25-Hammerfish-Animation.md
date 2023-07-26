---
title: "Hammerfish Animation"
date: 2023-07-25T15:34:30-04:00
categories:
  - blog
tags:
  - Houdini
  - 
---

This is a part of some early testing I've been doing for creature animations, meant for a small game that's been knocking around in my head. The idea is to have several animals roaming about the environment. I'm just one person so a good option for accomplishing that would be to do all the modeling inside Houdini, rely on CHOPs-driven animation, and a bit of simulation sprinkled throughout to quickly give life to each of the creatures. After modeling and animating, I export them using the VAT output SideFX ships, allowing for much more fauna than what would be possible with bone-based animations. In my mind, the advantage of this approach is the ability to animate while modeling, then tweak and add details while retaining those already created animations. This serves as a brief walkthrough of the setup for this "Hammerfish". At the bottom of the page, you'll find an image of the full network.


<img src="https://bakedveg.github.io/portfolio/assets/gif/HammerfishAnimLoopAlpha.gif">

<img src="https://bakedveg.github.io/portfolio/assets/gif/HammerfishAnimTopAlpha.gif">


<br>
<br>

<div style="clear: both;">
    <h2>Body</h2>
    <p>I started with a sphere, grouped both ends and used soft transforms to get the desired bell shape. Then smoothed the result.</p>
</div>
<img src="https://bakedveg.github.io/portfolio/assets/gif/BodyCreationWalkthroughAlphaFixed.gif">


<div style="clear: both;">
    <h2>"Hammers"</h2>
    <p>I find it easiest to start with curves when there's a specific silhouette I'm looking for. This is extruded and then subdivided. The top and bottom faces are grouped and transformed to give a rounder appearance after its been converted to a VDB, back to polygons, and smoothed. The result is mirrored to give that hammerhead-like shape. Little details are added to it afterward. </p>
</div>
<img src="https://bakedveg.github.io/portfolio/assets/gif/HammerCreationWalkthroughAlpha.gif">


<div style="clear: both;">
    <h2>Combine Body and "Hammers"</h2>
    <p>The pieces are merged by converting to VDB, then back to polys. I get a useable topology using Quadremesher, before splitting the mesh into one "quadrant". All my references were squids with these beautiful patterns. Some of them had a nice symmetry to them, and in pursuit of that look, I felt it best to have mirrored UVs. This made it easier to texture in Substance Painter and gave me a higher resolution for details.   </p>
</div>
<img src="https://bakedveg.github.io/portfolio/assets/gif/CombinationWalkthroughAlpha.gif">


<div style="clear: both;">
  <div style="float: right; margin-right 1em;">
    <img src="https://bakedveg.github.io/portfolio/assets/gif/VellumTentacleWalkthroughAlpha.gif">
  </div>
  <div>
    <h2>Vellum Tentacles</h2>
    <p>All of the animations (including the main body) are done using transforms with parameters driven by a CHOPs node so it's easily visualized, tweaked, and in sync. For the tentacle animation, I copied lines to a disc, ran that through a vellum hair sim, and swept the resulting curves. Details were added by copying planes and tentacle "feet" to points I grouped after the vellum sim. The sweep node generated UVs for the curves, and the other pieces were done separately. All of the UVs were then quickly rearranged manually for easier texturing.  </p>
  </div>
</div>

<br>
<br>


<div style="clear: both;">
    <h2>Final Assembly</h2>
    <p>Both pieces were then moved into position using transforms.</p>
</div>
<img src="https://bakedveg.github.io/portfolio/assets/images/FinalAssembly.png">



<div style="clear: both;">
  <div style="float: right; margin-right 1em;">
  </div>
  <div>
    <h2>Texturing</h2>
    <p>I used "quick material" nodes throughout so that when I exported to Substance Painter for texturing, the texture sets were filled out. Substance recognizes different name attributes as separate meshes and a shop_materialpath name as a texture set.</p>
  </div>
</div>

<img src="https://bakedveg.github.io/portfolio/assets/images/FinalTextured.png">



<div style="clear: both;">
  <div style="float: right; margin-right 1em;">
  </div>
  <div>
    <h2>Full Network</h2>
    <p></p>
  </div>
</div>

<img src="https://bakedveg.github.io/portfolio/assets/images/HoudiniHammerfishGeoNetwork.png">
