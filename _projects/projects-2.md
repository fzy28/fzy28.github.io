---
title: "Volumetric Path Tracing"
excerpt: "Implement Volumetric Path Tracing for both homogeneous and heterogeneous volumes. <br/><img src='/images/volpath_5_cbox.png' width='300px'>"
collection: projects
---
The main difficulty lying in implementing heterogeneous volumes. Since the transmittance obtained from the ODE equation is an integral in this case, a clever technique called null-scattering is required to solve this problem.
Additionally, implementing multiple importance sampling in this scenario is also a challenging problem.

<br/><img src='/images/hetvol.png' alt='Monochromatic heterogeneous volume'>
<p>Monochromatic heterogeneous volume<p>
<br/>
<img src='/images/colored_smoke.png' alt='Colored heterogeneous volume'><p>Colored heterogeneous volume<p>
<br/><img src='/images/scene.png' alt='my own scene'>
<p>My own scene<p>

My scenes are all created using Blender.