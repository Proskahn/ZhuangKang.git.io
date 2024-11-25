---
layout: post
title: Computed tomography and Bregman method
date: 08.09.2023
description: This report focus on computed tomography. # Add post description (optional)
img: image4.jpg # Add image post (optional)
---

Tomographic image reconstruction probably stands as one of the most important inverse problems, with a mathematical history more than 100 years.

The analytical approach, initially proposed by Cormack and currently employed in modern commercial CT scan machines, relies on Fourier transforms and theoretically promises perfect image recovery without any loss of information. Nonetheless, practical limitations such as the inability to acquire all projections from every angle and sensitivity to noise necessitate alternative methods to enhance CT reconstruction performance.

Recognizing the drawbacks of the analytical approach and the need to address these challenges, the optimization-based approach emerges as a viable alternative, having actually appeared prior to the analytical approach. In fact, the first CT scanner, designed in the late 1960s by Godfrey Hounsfield, employed an approach grounded in linear algebra and matrix theory to generate images from machine readings. Algorithms that adhere to this perspective are known as Algebraic Reconstruction Techniques (ART). However, due to its slow convergence and challenges in computer implementation, it was eventually replaced by the analytical approach.

Recent years have witnessed a resurgence of interest in optimization- and variation-based image reconstruction models and their associated algorithms, particularly in the context of sparse-view CT. These approaches have experienced remarkable growth due to their ability to reduce the number of scanning views while either maintaining or improving image quality, addressing the challenge of robust image reconstruction in situations with limited data. This is achieved by incorporating prior knowledge to regularize the underdetermined problem.

In parallel with the development of reconstruction models, a multitude of novel algorithms have been proposed to solve the optimization problem. Among those algorithms Bregman method is recognized for its rapid convergence speed and proficiency in non-smooth optimization. In the following reoprt we discuss the application of Bregman method in computed tomography.

https://drive.google.com/file/d/10bOBWi_OokC1mFp0x_yiHud2DALn79ub/view?usp=share_link