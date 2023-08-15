---
title: "HEM's Last Visitor: HDAs"
date: 2023-07-25T15:34:30-04:00
categories:
  - blog
tags:
  - Houdini
  - Substance
---

I knew before I started the project that the He Art Museum would be the backdrop for the plant animation, but as I continued to piece things together, this idea kept creeping in about what these large public structures would look like if we weren't around. I thought about how plants would surely be some of the last visitors to our monuments. So after completing the structure, I set out to create a few tools to quickly "dress" every surface with a happy little visitor. In this brief breakdown, I'll walk you through a few of the tools I created to speed things along.

<iframe width="560" height="315" src="https://www.youtube.com/embed/RWa-IMMJHwo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<div style="clear: both;">
    <h2></h2>
    <p></p>
</div>
<br>
<br>
<br>

<div style="clear: both;">
    <h2>Ivy Scattering</h2>
    <p>The scene uses four instances of the same ivy scatter HDA. The available parameters are simple as I either wanted ivy hanging from walls or under the stairs. The main points are an easy-to-understand density parameter, size and rotation control, the all-important seed, and a toggle to populate inside faces. This last parameter is a group based on normals facing the origin.</p>
</div>

<iframe width="560" height="315" src="https://www.youtube.com/embed/uS5XyUBHr0Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>



<div style="clear: both;">
    <h2>Fern/Leaf Scattering</h2>
    <p>Ferns and leaves were scattered using the same tool. It's essentially the ivy scatter HDA but with a couple of extra parameters. This tool was meant to scatter on both the main floor and staircases, as such it has a scatter exclusion scale so I didn't have any clipping into the main plant, and a drop-down menu for selecting an area to scatter on. The incoming meshes from Unreal are separated based on normal orientation and scatter location is selected after that.</p>
</div>

<iframe width="560" height="315" src="https://www.youtube.com/embed/Jdz42H3bdbU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>



<div style="clear: both;">
    <h2>Vine Generation</h2>
    <p>Text</p>
</div>

<iframe width="560" height="315" src="https://www.youtube.com/embed/TagYh-tuoCM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>



<div style="clear: both;">
    <h2>Bonus: Materials Overview</h2>
    <p>Text</p>
</div>

<iframe width="560" height="315" src="https://www.youtube.com/embed/_fWKdqvzUfM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>





<div style="clear: both;">
    <h2></h2>
    <p>If you have any questions or comments don't hesitate to reach out. My contact information is linked on the left and at the bottom. Til next time!</p>
</div>
