---

layout: post
title: Bregman Learning(Thesis)
date: 30.09.2024
description: How to reduce the number of active parameters all along the training?
img: Figure6.png
---

Bregman method starts from a smooth initial condition (often zero) and progressively recovers large-scale features first, followed by finer details. 

A question is, how Bregman iteration behaves in neural network training?Theoretically, after applying the $$\ell_1$$-regularization and starting from sparse initialization, neural networks are expected to preserve sparsity because, in the early iterations, only parameters with large gradient norms are updated. This thesis investigates this phenomenon from both theoretical and practical perspectives.


Click the link below to read the full article.

https://drive.google.com/file/d/1TMxS9mZLM1OW4AWvKIVFT9cLLTyAhmi8/view?usp=share_link