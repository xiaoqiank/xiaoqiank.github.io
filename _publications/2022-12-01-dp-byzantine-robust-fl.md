---
title: "Differentially Private Byzantine-Robust Federated Learning"
collection: "publications"
category: "manuscripts"
permalink: "/publication/2022-dp-byzantine-robust-fl/"
date: "2022-12-01"
authors: "Xu Ma, **Xiaoqian Sun**, Yuduo Wu, Zheli Liu, Xiaofeng Chen, and Changyu Dong."
venue: "IEEE Transactions on Parallel and Distributed Systems (TPDS)"
year: 2022
volume: 33
issue: 12
pages: "3690–3701"
doi: "10.1109/TPDS.2022.3167434"
---

<!-- Abstract transcribed from the author's local published PDF; only PDF line wrapping and typographic ligatures normalized. -->

Federated learning is a collaborative machine learning framework where a global model is trained by different organizations under the privacy restrictions. Promising as it is, privacy and robustness issues emerge when an adversary attempts to infer the private information from the exchanged parameters or compromise the global model. Various protocols have been proposed to counter the security risks, however, it becomes challenging when one wants to make federated learning protocols robust against Byzantine adversaries while preserving the privacy of the individual participant. In this article, we propose a differentially private Byzantine-robust federated learning scheme (DPBFL) with high computation and communication efficiency. The proposed scheme is effective in preventing adversarial attacks launched by the Byzantine participants and achieves differential privacy through a novel aggregation protocol in the shuffle model. The theoretical analysis indicates that the proposed scheme converges to the approximate optimal solution with the learning error dependent on the differential privacy budget and the number of Byzantine participants. Experimental results on MNIST, FashionMNIST and CIFAR10 demonstrate that the proposed scheme is effective and efficient.
