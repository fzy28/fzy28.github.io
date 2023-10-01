---
title: "My single scatter NeRF"
excerpt: " Attempted to implement Single Scatter NeRF. I explored various network structures and representations of phase functions.<br/><img src='/images/CSE_272.jpg'>"
collection: projects
---

In this assignment, I attempted to implement Single Scatter NeRF. I explored various network structures
and representations of phase functions. In conclusion, I believe that the most significant challenge in implementing Single Scatter NeRF is learning the geometry. I tried multiple approaches to address this issue, which will be discussed in detail later in the report.

Firstly, I implemented an acceleration structure for my NeRF. With reference to Instant-NGP, I integrated
Hashcoding and occupancy grid into my NeRF implementation, utilizing the NeRFacc framework. Additionally, I employed PyTorch and tiny-cuda-nn for training, which significantly increased the training speed. As a result, I achieved 120-130 iterations per second (iters/s) on the original NeRF dataset. In the implementation of Single Scatter NeRF, it also substantially accelerated the ray marching process. Even if fully considering the
scattering of each ray sample, it managed to achieve 6-10 iters/s, making the training time acceptable.

Secondly, I experimented with different Single Scatter NeRF models, including variations in network
structure and loss function. The primary distinctions among these models lie in the representation of phase functions: one approach uses physically meaningful phase functions from computer graphics, while the other treats phase functions as a separate network.

In addition, I used Blender to generate a series of datasets specifically designed for Single Scatter NeRF
testing purposes.

This idea is actually implemented by a paper called [NeMF: Inverse Volume Rendering with Neural Microflake Field](https://arxiv.org/abs/2304.00782#:~:text=Recovering%20the%20physical%20attributes%20of,essential%20for%20photo%2Drealistic%20rendering.).
If you want, you may check my [full report here](https://drive.google.com/file/d/1kaYQGENe8mTQF7u29UlFQ1i6DiH4WwyT/view?usp=drive_link).
