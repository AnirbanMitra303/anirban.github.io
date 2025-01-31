---
layout: post
title: "Random Matrix Theory"
subtitle: "The beautiful world of Wigner"
date: 2021-08-29
#googlewebfonts: Gloria+Hallelujah
---

<!--<div style="text-align: justify" style="font-size:1.2em">-->
My first encounter with Wigner's name was when I was suggested to read the Wigner-Ville distribution and Gabor transform during my brief work on a signal processing project three years back. The project was short and I did not care to make any in-depth venture into Wigner's work. A couple years after that I had started to read on random matrix perturbations when I started come across terms such as **Wigner matrix**, **Wigner's surmise**, **Wigner semi-circle law**, and so on. Now this piqued my interest because I had heard of Wigner before. Upon looking up the Wikipedia page I found that Eugene Wigner was a physicist (well, primarily) and a Nobel laureate (1963)! <br>
Only recently I had the pleasure of coming across the <em>The Oxford Handbook of Random Matrix Theory</em> (OH-RMT), and I am so very thankful to myself for digging on this subject in our library catalogue. This blog (hopefully a series) will be based on this book and few external supportive research/reading that I conduct. So, as I read along, start to understand the origins and implications  of **Random Matrix Theory** (RMT) (and get my mind blown), I will continue writing on this. This is such an ocean of knowledge, I will be extremely happy if I can digest even a drop of it.<br>  
It is indeed very hard (as a novice) to decide from where to begin. Let me start by defining some matrices and matrix ensembles. Let us say $$\mathbf{W}$$ is an $$n$$-dimensional symmetric matrix with the $$(i,j)$$-th entry denoted by $$W_{ij}$$. $$\mathbf{W}$$ is a Wigner matrix if it satisfies the following conditions:
<ul>
    <li style="font-size:1.2em">The entries are independent upto symmetry. That is $W_{ij}$ are independent for all $1 \le i\le j \le n$.</li>
    <li style="font-size:1.2em">The diagonal entries are independent and identically distributed (i.i.d.) and the entries in the lower triangle are also i.i.d and also independent of the diagonal entries.</li>
    <li style="font-size:1.2em">The expected values of the squares of entries are finite, i.e. $\mathbb{E}\left(W_{ij}^{2}\right) < \infty$.</li>
    <li style="font-size:1.2em">All entries are centered.</li>
</ul>
Next, let us learn about some matrix ensembles, more specifically Gaussian ensembles. The name <em>Gaussian ensemble</em> suggest that it has something to do with the Gaussian or Normal distribution. We will see that in a bit, but why "ensembles"? Well, to study asymptotics (or convergence) we most obviously need the number of "virtual" copies to be large or in this case we need the dimension of matrix to be large. The entries of a Gaussian ensemble, $$\mathbf{H}_{n}$$ (the subscript $$n$$ denotes the dimension of the matrix as well as hinting at the fact that a growing $$n$$ is used to study asymptotics), are independent upto symmetry and have the following probability density: 

$$
\begin{align*}
  f(\mathbf{H}) = \frac{1}{Z_{GE}}\exp\left(-\frac{n\beta}{4}\operatorname{tr}(\mathbf{H}^{2})\right)
\end{align*}
$$

$$Z_{GE}$$ is the normalizing constant which depends on the type of ensemble. Three types of ensembles are typically considered: Gaussian Orthogonal Ensemble (GOE), Gaussian Unitary Ensemble (GUE) and Gaussian Simplectic Ensemble (GSE). So the density is essentially proportional to an exponent. Now the exponent depends on the term $$\beta$$, called the Dyson index which takes values $$1$$ for GOE, $$2$$ for GUE and $$4$$ for GSE. (OH-RMT has its foreword written by Freeman Dyson!) 
<ul>
    <li style="font-size:1.2em"> GUE is defined for Hermitian matrices ($H_{ij} = \overline{H_{ji}}$) so that $\mathbf{H} = \frac{\mathbf{A}+\overline{\mathbf{A}}}{\sqrt{2}}$ with $A_{ij} \sim \mathcal{N}(0,\frac{1}{2}) + i \mathcal{N}(0,\frac{1}{2})$ for $i\neq j$ and $A_{ii} \sim \mathcal{N}(0,1)$.</li>
    <li style="font-size:1.2em"> GOE is defined for real symmetric matrices ($H_{ij} = H_{ji}$) so that $\mathbf{H} = \frac{\mathbf{A}+\mathbf{A}^{\top}}{\sqrt{2}}$ with $A_{ij} \sim \mathcal{N}(0,1)$ for $i\neq j$ and $A_{ii} \sim \sqrt{2}\mathcal{N}(0,1)$.</li>
    <li style="font-size:1.2em"> GSE is defined for quaternionic Hermitian matrices $\mathbf{H}$. Quaternions are basically extension of the complex number system and just as in GUE the off-diagonal entries are associated with one real and one imaginary part, in GSE it will one real element and three quaternions.</li>
</ul>
The Dyson index basically counts the number of real elements associated with each entry of the matrix. <a href="/blog/2022/05/09/Wigner-part-two">continued here</a>
{: .text-justify}
<!--</div>-->