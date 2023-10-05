---
layout: single
title:  "Draft Post"
header:
  teaser: "unsplash-gallery-image-2-th.jpg"
categories:
  - Jekyll
tags:
  - edge case
---
$$
\mathbb{E}\left(\prod_{i=1}^kz_i^{N(A_i)}\right)
$$

$$
=\mathbb{E}\left(\mathbb{E}\left(\prod_{i=1}^kz_i^{N(A_i)}\Bigg\vert N=\sum_{i=1}^kN(A_i)\right)\right)
$$

$$
=\mathbb{E}\left(\left(\sum_{i=1}^kp_iz_i\right)^N\right)
$$

where $p_i=F(A_i)$.

Suppose $N\sim \mathcal{NB}(\alpha,\mu)$, the PGF of $N$ is

$$
P_N(z)=\left(1+\mu(1-z)\right)^{-\alpha}
$$

Substitute $z=\sum_{i=1}^kp_iz_i$ into the above expression, we have

$$
\mathbb{E}\left(\prod_{i=1}^kz_i^{N(A_i)}\right)
$$

$$
=\left(1+\mu\left(1-\sum_{i=1}^kp_iz_i\right)\right)^{-\alpha}
$$

$$
=\left(1+\mu\left(\sum_{i=1}^kp_i-\sum_{i=1}^kp_iz_i\right)\right)^{-\alpha}
$$

$$
=\left(1+\mu\sum_{i=1}^kp_i(1-z_i)\right)^{-\alpha}
$$

$$
=\left(1+\mu\sum_{i=1}^kF(A_i)(1-z_i)\right)^{-\alpha}
$$