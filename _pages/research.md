---
permalink: /research/
title: "Research"
author_profile: true
---

My PhD work asks how genome sequence alignment can run efficiently on spatial accelerators that are available off the shelf today, such as the AMD Versal ACAP AI Engine array, AMD NPUs and Tenstorrent devices.

Data orchestration across processing elements
------
Spatial accelerators pair many small processing elements with explicit data movement. I study how to map the data flow of alignment kernels onto these arrays so that processing elements stay busy instead of waiting on memory. On the AI Engine this means optimizing kernels for its VLIW and SIMD vector processors in C and C++, and exploring a generic data mapping model for dynamic programming algorithms across CPU, FPGA and AI Engine.

Comparing alignment algorithm families
------
I evaluate three families of alignment algorithms on the same architecture and quantify where each is strong or weak:

* dynamic programming (Smith-Waterman-Gotoh, including striped and inter-sequence variants),
* bit-parallel methods (Bitap),
* wavefront methods (WFA).

Throughput is measured in GCUPS (giga cell updates per second) and compared against energy efficiency (performance per watt).

Sequence-to-graph alignment
------
I am also exploring how converting sequences to graphs, and applying graph techniques to the result, can further optimize alignment.

Related industry work
------
Memory-centric computing (processing-in-memory, processing-using-memory, non-volatile memory), heterogeneous CPU, GPU and NPU scheduling, and roofline analysis for AMD GPUs.
