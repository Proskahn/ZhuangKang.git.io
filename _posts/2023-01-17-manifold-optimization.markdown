---

layout: post
title: image segmentation via manifold optimization
date: 17.01.2023
description: This is a introduction of how to apply manifold optimization theory to image segmentation. # Add post description (optional)
img: WechatIMG143.jpg
---
Active contour models, have been widely used for segmentation problem, aim to extract the boundary of an area contained in the image. The main idea is minimizing an energy defined on curves, that the minima will be closed to the desired boundary.

Let $$I$$ denotes the intensity of an image on a domain $$\Omega \subset \mathbb{R}^2$$. Active contour model is defined as a functional $$E_{snake}$$ applied to a curve in the image domain $$\Omega$$. For example, 
\begin{equation}\label{eq1}
E_{snake}=\int_0^1E(v(s))=\int_0^1E_{int}(v(s))+\int_0^1E_{image}(v(s))+\int_0^1E_{con}(v(s)).
\end{equation}


$$E_{int}$$: Internal energy of the spline due to tension and rigidity.

\begin{equation}\label{eq2}
E_{int}=\alpha(s)\lvert dv/ds\rvert^2+\beta(s) \lvert d^2v/ds^2 \rvert.
\end{equation}

$$E_{image}$$: Energy comes from image force and higher-level image understand process.
\begin{equation}
E_{image}=-\lvert \nabla I(v(s))\rvert^2.
\end{equation}
$$E_{con}$$: External constrain force.

Minimization of the energy is naturally an optimization problem on the space of closed curves. In the following report we consider a specific way to define a Riemannian manifold structure(infinite-dimensional) on closed curves and explore the possibilities to do optimization on this manifold.

https://drive.google.com/file/d/1FEOTzcrGcS5kZiQYdV0L2bUReKfRr77A/view?usp=share_link