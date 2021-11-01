
WebGL Forward+ and Clustered Deferred Shading
======================

**University of Pennsylvania, CIS 565: GPU Programming and Architecture, Project 5**

* Shubham Sharma
  * [LinkedIn](www.linkedin.com/in/codeshubham), [personal website](https://shubhvr.com/).
* Tested on: Windows 10, i7-9750H @ 2.26GHz, 16GB, GTX 1660ti 6GB (Personal Computer).
*GPU Compute Capability: 7.5

### Live Online

[![](img/thumb.png)](http://TODO.github.io/Project5-WebGL-Forward-Plus-and-Clustered-Deferred)

### Demo Video/GIF

[![](img/video.png)](TODO)

### Overview

This project highlights the performance differences between Forward, Forward+ clustered and Deferred clustered shading schemes. 
- Forward : Implementation of Forward shading in this project has been updated to calculate the visible object Mesh once and iterating through all the lights in the scene to shade the visible mesh or vertices.
-  Forward+ : The Scene is divided into tiled frustum clusters, which expand along the X, Y and Z axes. The Scene objects are shaded only iterating through the lights which affect them or the lights which affect the clusters in which the object lies in.
- Deferred Clustered : This required multiple passes of the OpenGL draw pipeline. Scene information is stored as G Buffers in the first pass and the scene is shaded using the same cluster methodology as Forward+ Shading.    

### Performance Analysis 


### Credits

* [Three.js](https://github.com/mrdoob/three.js) by [@mrdoob](https://github.com/mrdoob) and contributors
* [stats.js](https://github.com/mrdoob/stats.js) by [@mrdoob](https://github.com/mrdoob) and contributors
* [webgl-debug](https://github.com/KhronosGroup/WebGLDeveloperTools) by Khronos Group Inc.
* [glMatrix](https://github.com/toji/gl-matrix) by [@toji](https://github.com/toji) and contributors
* [minimal-gltf-loader](https://github.com/shrekshao/minimal-gltf-loader) by [@shrekshao](https://github.com/shrekshao)
