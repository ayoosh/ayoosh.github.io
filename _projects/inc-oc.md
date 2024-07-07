---
layout: page
title: INC-OC
description: Reconciling Predictability and Coherent Caching
img: assets/img/inc-oc.png
importance: 3
category: 
related_publications: true
publications: bansal2020reconciling
selected: true
---

<div style="text-align: justify;">

<p>
Real-time and cyber-physical systems
need to interact with and respond to their physical
environment in a predictable time. While multicore
platforms provide incredible computational power and
throughput, they also introduce new sources of unpredictability.
Large fluctuations in latency to access data
shared between multiple cores is an important contributor
to the overall execution-time variability. In addition
to the temporal unpredictability introduced by
caching, parallel applications with data shared across
multiple cores also pay additional latency overheads
due to data coherence.
</p>

<p>
Analyzing the impact of data coherence on the worst-case
execution-time of real-time applications is challenging
because only scarce implementation details
are revealed by manufacturers. This work introduces
application-level control for caching data at different
levels of the cache hierarchy making latency to access data present in
caches independent of the coherence state. 
A new memory type Inner-NonCacheable, Outer-Cacheable (INC-OC) is
implemented with OS and architectural support on the Gem5 simulator.
Worst-case execution time for a single memory write request
is reduced by 52% while benchmark evaluations show that
the proposed technique has a minimal impact on average
performance.
</p>

</div>

<br>