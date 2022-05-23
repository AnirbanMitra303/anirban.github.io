---
layout: post
title: "Random Matrix Theory part 2"
subtitle: "The beautiful world of Wigner -- 2"
date: 2022-05-09
#googlewebfonts: Gloria+Hallelujah
---

<!--<div style="text-align: justify" style="font-size:1.2em">-->
Nearly a year has passed since I continued writing. I read some, but exams came and went and other stuff made me too preoccupied to make a coherent write up. By now I have forgotten a lot of what story I wanted to tell. I also run the risk of copying or plagiarising from different sources like Wikipedia, but mainly from OH-RMT. While blogs are supposed to be for sharing one's original thoughts, I think I will give myself a break here and just say that I am writing this to trach myself, and to create a resource for my future self.<br>
I ended the <a href="/blog/2021/08/29/Wigner-part-one">previous blog</a> by briefly stating the Gaussian ensembles. One can easily notice that they are special cases of Wigner matrices. It would also make sense to signify the previously stated Dyson index (in context of probability density) to the eigen value distribution of Gaussian ensembles. I will now shift my focus only to GOE, becasue it serves my learning purpose for now. GUE might also have been of interest, but GSE is out of my brain's reach right Suppose $$\lambda_{1},\lambda_{2},\cdots,\lambda_{n}$$ are the eigen values of an $$n$$-dimensional Gaussian ensemble. Then the joint probability distribution of the eigen values is given by

$$
\begin{align*}
  f(\lambda_{1},\lambda_{2},\cdots,\lambda_{n}) = \frac{1}{Z_{GE}^{'}}\exp\left({-\beta \sum_{l=1}^{n}\lambda_{l}^{2}/4}\right)\prod_{i<j}|\lambda_{i} - \lambda_{j}|^{\beta}.
\end{align*}
$$

Here, $$\beta$$ is the Dyson index as defined before. I now realize that this indeed is closely related with canonical correlation. For GOE the normalizing constant $$Z_{GE}^{'}$$ is related to the multivariate gamma function and the corresponding characteristic vectors are independently distributed as the conditional Haar invariant distribution (Th. 13.3.5, T.W. Anderson, An introduction to multivariate statistical analysis). I will next state Wigner's surmise, the semicircle law, and plan to touch upon Marcenko-Pastur law and Tracy-Widom distribution. (<em>to be continued</em>...)
