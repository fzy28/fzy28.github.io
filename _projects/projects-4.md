---
title: "Parallel Computation course projects"
excerpt: "There were three assignments in the Parallel Computation course, each implementing matrix multiplication on different platforms: CPU, GPU, and MPI-distributed tasks."
collection: projects
---

The first assignment implemented matrix multiplication on CPU using C language, with a focus on cache
locality and SIMD acceleration. The [blislab tutorial](https://github.com/flame/blislab/blob/master/tutorial.pdf) was referenced, achieving 100% performance based
on the Blas benchmark.
The second assignment implemented matrix multiplication on GPU using C++ and CUDA, referring to
the [CUTLASS](https://developer.nvidia.com/blog/cutlass-linear-algebra-cuda/) algorithm. It achieved 80% performance compared to the CUblas benchmark library.
The third assignment was implemented on Expanse, a high-performance computing cluster at the school,
using MPI to distribute the matrix multiplication tasks to multiple processors.