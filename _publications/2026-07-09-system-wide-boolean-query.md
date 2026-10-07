---
title: "A Searchable Encryption With System-Wide Forward and Backward Security Supporting Boolean Query"
collection: "publications"
category: "manuscripts"
permalink: "/publication/2026-system-wide-boolean-query/"
date: "2026-07-09"
authors: "Guiyun Qin, **Xiaoqian Sun**, Fangzhou Yi, Siyi Lv, Xiaoxin Du, Zheli Liu, and Xiaofeng Chen."
venue: "IEEE Transactions on Dependable and Secure Computing (TDSC)"
year: 2026
volume: 23
issue: 4
pages: "9302–9315"
doi: "10.1109/TDSC.2026.3692543"
---

<!-- Abstract transcribed from the author's local published PDF; only PDF line wrapping and typographic ligatures normalized. -->

Gui et.al (S&P 2023) first proposed an attack exploiting vulnerabilities in document retrieval to reconstruct queries. In response, they (PETS 2024) introduced the first searchable encryption (SE) scheme supporting system-wide security using frequency bucketization and obfuscation. However, it only supports single-keyword retrieval and has limitations in applicability and efficiency. Multi-keyword retrieval, widely used in practice, is also susceptible to system-wide leakage-abuse attacks, with no effective defense mechanisms available. We propose a secure system-wide SE scheme that enhances system security and scalability without compromising practicality. For security, we introduce a volume bucketization technique to protect the volume of retrieved documents. For efficiency, it significantly reduces computational and communication complexity and minimizes the update rounds. Building on this foundation, we introduce the first multi-keyword retrieval scheme supporting system-wide security, using dynamic bitmap and adaptive volume hiding techniques. It demonstrates low overhead and effectiveness in multi-keyword search scenarios. Experiments show that, on large-scale datasets, our method outperforms existing solutions by at least 100 × in write-back and update efficiency. Client-side cache overhead is reduced by 78%. In the multi-keyword retrieval, a Boolean query involving 8 keywords takes approximately 454.78 ms.
