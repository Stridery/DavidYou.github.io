---
title: "Light Tracing Project"
excerpt: "In this project I independently designed a light tracing project and a octree accelerate strategy.<br/><img src='/images/!balls.png'>"
collection: portfolio
---

The fundamental idea of light tracing is to send rays from the camera through each pixals into the environment and see what it hits. If the ray hits an object, calculate its color though its own texture, the light source's color and angle, and the angle between the reflection light and the light source. Once the original color of the object is abtained, repeat the process with the reflection light to see reflection color of the pixal, and add it on the original color.<br>
<br/><img src='https://github.com/Stridery/DavidYou.github.io/blob/master/images/LTconcept.png'><br>
And to accelerate the process, I focused on shortening calculation needed to see what the ray hits.<br>
The original plan was to check every object in the scene, and choose the one with the sortest distance. This is obviously extremely inefficiant. My accelerate plan is to create a smallest box possible to cover all objects in the environment. Divide the box into 16 smaller boxes, and divide each of them into 16 even smaller boxes, thus build a three-layer octree structure, and record the objects each smallest box includes.<br>
<br/><img src='https://github.com/Stridery/DavidYou.github.io/blob/master/images/motherbox.png'><br/><img src='https://github.com/Stridery/DavidYou.github.io/blob/master/images/sonbox.png'><img src='/images/box.png'><br>
<br/><img src='https://github.com/Stridery/DavidYou.github.io/blob/master/images/octree.png'><br>
When checking what the ray hits, check the smallest boxes the ray hits, and simply check whether the ray hits the objects in the boxes hit by the ray. A maximum 9 boxe out of the 64 can be hit, therefore theoretically this strategy can accelerate this process around 8 times. <br>

More detailed elaboration can be found in my paper and my repository. Here are some pictures rendered.<br>
<br/><img src='https://github.com/Stridery/DavidYou.github.io/blob/master/images/!teapot.png'><br>
<br/><img src='https://github.com/Stridery/DavidYou.github.io/blob/master/images/!rings.png'><br>
<br/><img src='https://github.com/Stridery/DavidYou.github.io/blob/master/images/!balls.png'><br>
