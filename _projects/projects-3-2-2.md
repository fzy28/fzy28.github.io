---
title: "AliCloth Rendering project"
excerpt: "This is my undergraduate graduation project, which was used in a clothing rendering project at Alibaba.<br/><img src='/images/cloth.png' width='550px'>"
collection: projects
---

My project introduces an algorithm to enhance the rendering effects of common fabric models. By making reasonable predictions and augmenting the data, we aim to render images of fabric that align with reality. I referenced the micro-cylinder model and proposed a BSDF formula to simulate the radiance of different fabrics in various directions of emission. As for the representation information of the common fabric model, I decomposed it into geometric and probabilistic information. Part of this is used to reconstruct the tangent map, while another part is utilized to fit certain parameters in the BSDF formula. Parameters that are challenging to derive from the fabric model information will be obtained through prior knowledge.

A comparison between my model and the original model. The first row is the original, and the second row is after enhancement.

<br/><img src='/images/1.png'>

The fabric is continuously magnified along the center, displaying the details of the fabric.

<br/><img src='/images/2.png'>

Practical application results

<br/><img src='/images/3.png'>

