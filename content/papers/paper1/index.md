---
title: "Kubism: Disassembling and Reassembling K-Means Clustering for Mobile Heterogeneous Platforms"
date: 2025-06-13
tags: ["k-means","heterogeneous computing","mobile platforms","embedded"]
author: ["Seondeok Kim","Sangun Choi","Jaebeom Jeon","Junsu Kim","Minseong Gil","Jaehyeok Ryu","Yunho Oh"]
description: "An English summary and metadata for 'Kubism', a software technique that improves K-means performance on mobile heterogeneous platforms."
summary: "Kubism disassembles and reassembles the K-means algorithm to better utilize CPU and GPU resources on mobile heterogeneous platforms, achieving up to 2.65× speedup per iteration and an average 1.23× end-to-end improvement on NVIDIA Jetson Orin AGX."
cover:
    image: "paper1.png"
    alt: "Kubism overview"
    relative: false
doi: "10.1145/3735452.3735537"
---

##### Summary (English)

This paper presents Kubism, a software approach designed to improve the performance
and resource utilization of K-means clustering on mobile heterogeneous platforms
(e.g., NVIDIA Jetson Orin AGX). Traditional parallel K-means implementations often
underutilize GPU warps and leave CPU resources idle. Kubism addresses these
inefficiencies by disassembling the K-means algorithm into finer-grained tasks and
reassembling them to achieve balanced, dynamic cooperation between CPU and GPU.

Key techniques include:

- Reordering operations to avoid unnecessary work
- Balancing workloads across CPU and GPU to reduce idle time
- Dynamically adjusting task allocation using runtime performance metrics
- Reconfiguring processing units to minimize waiting and synchronization overhead

Combined, these strategies lead to significant improvements: up to 2.65× speedup
in individual clustering iterations and an average 1.23× improvement in overall
end-to-end execution time compared to prior work, as measured on a Jetson Orin AGX
evaluation platform. The paper details the design, implementation, and empirical
evaluation of Kubism.

---

##### Download & Original

- ACM page: https://dl.acm.org/doi/10.1145/3735452.3735537
- PDF: https://dl.acm.org/doi/pdf/10.1145/3735452.3735537

---

##### Copyright note

The full text of the paper is available from the ACM Digital Library and is
subject to ACM copyright. This page provides an original English summary and
metadata only; consult the ACM PDF for the complete article.
