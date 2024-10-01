---
title: "Robust Sparse Mean Estimation via Incremental Learning"
collection: publications
category: conferences
permalink: /publication/robust
citation: "Jianhao Ma, Rui Ray Chen, <b>Yinghui He</b>, Salar Fattahi, and Wei Hu" # authors
excerpt: ""
date: 2023-05-24
venue: "ICLR 2024 Workshop on Bridging the Gap Between Practice and Theory in Deep Learning"
# slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
paperurl: "https://arxiv.org/abs/2305.15276"
# citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

<figure>
  <img src="{{ site.baseurl }}/images/robust.jpg" alt="Robust Figure 1">
</figure>

In this paper, we study the problem of robust sparse mean estimation, where the goal is to estimate a $$k$$-sparse mean from a collection of partially corrupted samples drawn from a heavy-tailed distribution. Existing estimators face two critical challenges in this setting. First, they are limited by a conjectured computational-statistical tradeoff, implying that any computationally efficient algorithm needs $$\tilde{\Omega}(k^2)$$ samples, while its statistically-optimal counterpart only requires $$\tilde{O}(k)$$ samples. Second, the existing estimators fall short of practical use as they scale poorly with the ambient dimension. This paper presents a simple mean estimator that overcomes both challenges under moderate conditions: it runs in near-linear time and memory (both with respect to the ambient dimension) while requiring only $$\tilde{O}(k)$$ samples to recover the true mean. At the core of our method lies an incremental learning phenomenon: we introduce a simple nonconvex framework that can incrementally learn the top-$$k$$ nonzero elements of the mean while keeping the zero elements arbitrarily small. Unlike existing estimators, our method does not need any prior knowledge of the sparsity level $$k$$. We prove the optimality of our estimator by providing a matching information-theoretic lower bound. Finally, we conduct a series of simulations to corroborate our theoretical findings.
