---
title: "Can I Get More? An Incremental Inference Attack on Encrypted SQL"
collection: "publications"
category: "conferences"
permalink: "/publication/2026-incremental-inference/"
date: "2026-05-18"
authors: "**Xiaoqian Sun**, Ruiqi He, Yang Zhang, Siyi Lv, Guiyun Qin, Fangzhou Yi, Zheli Liu, and Xiaofeng Chen."
venue: "IEEE Symposium on Security and Privacy (S&P)"
year: 2026
pages: "1118–1137"
doi: "10.1109/SP63933.2026.00133"
---

<!-- Abstract transcribed from the author's local published PDF; only PDF line wrapping and typographic ligatures normalized. -->

Effective leakage-abuse attacks on encrypted SQL query schemes primarily focus on column equality leakage or cross-column equality leakage. However, these approaches fail to effectively leverage the joint distribution information among correlated columns that are often revealed in multi-attribute queries. This limitation leads to an underestimation of the actual security risks in real-world deployments.

This paper presents Anchor-Joint Attack, an incremental inference framework that more effectively exploits joint distribution leakage to achieve superior plaintext recovery. We design an anchor-based incremental strategy that first extracts a set of high-confidence ciphertext plaintext mappings from column equality leakage and treats them as anchors. Guided by these anchors, the framework then incrementally incorporates joint distribution information to expand the recovered mappings in an iterative manner. Moreover, we formulate the recovery procedure as an optimal transport problem based on the Earth Mover’s Distance (EMD), which naturally accommodates partial domain overlap and supports iterative error detection and correction. This design avoids explicitly constructing the full joint distribution in a single step, thereby maintaining high recovery rates, robustness, and efficiency even under incomplete leakage conditions.

Extensive experiments on real-world data demonstrate that our attack outperforms existing state-of-the-art methods. In the encrypted boolean query scenario, our method achieves an optimal value recovery rate of 71.68% and an optimal row recovery rate of 95.45%, surpassing the Jigsaw attack (Nie et al., USENIX’24) by approximately 3.5 × and 2.5 ×, respectively. In the encrypted join query scenario, our method attains an optimal value recovery rate of 97.4%, exceeding the attacks proposed by Hoover et al. (USENIX’24) by about 1.2 ×, while improving runtime by approximately 20×.
