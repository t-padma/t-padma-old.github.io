---
title: 'Discrete Derivative'
date: 2018-06-09
permalink: /posts/2018/06/discrete-derivative/
tags:
  - calculus
  - calculus of finite differences
  - continuous
  - derivative
  - difference operator
  - discrete
  - factorial expression
  - falling factorial
  - hiroshi yuki
  - math girls
  - raising factorial
  - richardson
---

I came across the following interesting question in the book <a href="https://www.maa.org/press/maa-reviews/math-girls" target="_blank" rel="noopener">"Math Girls" by Hiroshi Yuki </a>:

<blockquote>
<p>Develop a definition for the differential operator $\Delta$ in discrete space,corresponding to the definition of the differential operator D in the continuous space.</p>
</blockquote>

We know that derivative of a function f at point x is the rate at which f changes at the point x . Geometrically, derivative at a point x is the slope of the tangent to the function f at x where a tangent is the limit of the secant lines as shown below :

<img class="wp-image-11202 aligncenter" src="https://gaurish4math.files.wordpress.com/2018/06/capture5.png" alt="Capture5" width="516" height="449" />
  
But this happens only in the continuous world where x "glides smoothly" from one point to another. But this is not the case in a discrete world. In the discrete world there is nothing like "being close to each other". Hence we cannot use the earlier definition of bringing h arbitrarily close to x. In a discrete world we cannot talk about getting "close" to something but instead we can talk about being "next" to each other.

<img class="size-full wp-image-11203 aligncenter" src="https://gaurish4math.files.wordpress.com/2018/06/capture6.png" alt="Capture6" width="433" height="256" />

We can talk about the change in x as it moves from x to x+1 while f changes from f(x) to f(x+1). We do not need limits here, so the definition of "difference operator" (analogous to differential operator ) will be :

$\Delta f(x) = \frac{ f(x+1) - f(x) }{(x+1) - x} = f(x+1) - f(x)$

Hence to find derivative of a function, say $g(x) = x^2$ , it is easy to verify that $Dg(x) = 2x$ but $\Delta g(x) = 2x + 1$ (using definitions mentioned above)

Now, when will we be able to get the same derivative in both discrete and continuous worlds? I read a little about this question in math girls and a little more in <a href="https://archive.org/details/introductiontoca00rich" target="_blank" rel="noopener">"An introduction to the calculus of finite differences" by C.H.Richardson</a>.
<p>Calculus of differences is the study of the relations that exist between the values assumed by the function whenever the independent variable takes on a series of values in arithmetic progression.
  
Let us write f(x) as $f_x$ instead from now onwards. So $f(x+1) - f(x) = \Delta f(x) = f_{x+1} - f_x$. Using above definition we can prove the following for functions $U_x$ and $V_x$ :

1) $\Delta^{k+1} U_x = \Delta^{k} U_{x+1} - \Delta^{k} U_x$

2) $\Delta (U_x + V_x) = \Delta U_x + \Delta V_x$ (or) $\Delta^k (U_x + V_x) =\Delta^k U_x + \Delta^k V_x$

3) $\Delta^k (cU_x) = c \Delta^k U_x$

<blockquote>
<p><b>Theorem</b>. $\Delta^n x^n = n!$</p>
</blockquote>

<i>Proof.</i> $\Delta x^n = (x+1)^n - x^n = n\cdot x^{n-1} + \text{terms of degree lower than} (n - 1)$. Each repetition of the process of differencing reduces the degree by one and also adds one factor to the succession $n(n - 1) (n - 2) \cdots$. Repeating the process $n$ times we have $\Delta^k x^n = n!$.

<blockquote>
<p><b>Corollary 1.</b> $\Delta^n ax^n = a\cdot n!$</p>
<p><b>Corollary 2.</b> $\Delta^{n+1} x^n = 0$</p>
<p><b>Corollary 3.</b> If $U_x$ is a polynomial of degree n i.e. $U_x= a_0+ a_1 x + a_3 x + \ldots + a_n x^n$ , then $\Delta^n U_x = a_n\cdot n!$.</p>
</blockquote>

We call the continued products $U_x^{|n|} = U_x\cdot U_{x+1}\cdot U_{x+2} \cdots U_{x+(n-1)}$ and $U_x^{(n)} = U_x \cdot U_{x-1}\cdot U_{x-2}\cdots U_{x-(n-1)}$ as <b>factorial expressions</b>.

If $U_x$ is the function ax+b for some real numbers a and b, then the factorial forms we get by replacing $U_x$ by ax+b is $(ax+b)^{|n|} = (ax+b)\cdot(a(x+1)+b)\cdot (a(x+2)+b)\cdots (a(x+n-1)+b)$ and $(ax+b)^{(n)} =(ax+b)\cdot (a(x-1)+b)\cdot (a(x-2)+b)\cdots (a(x-(n-1))+b)$.
 
We define $(ax+b)^{|0|}$ and $(ax+b)^{(0)}$ as 1.
  
Using the above definition of factorial we can show the following :
  
(i) $\Delta (ax+b)^{(n)} = a\cdot n \cdot (ax+b)^{(n-1)}$
  
(ii) $\displaystyle{\Delta \frac{1}{(ax+b)^{|n|}} = \frac{-an}{(ax+b)^{|n+1|}}}$
  
When we consider the special case of a=1 and b=0, the factorial representations are called <b>raising</b> and <b>falling factorials</b> :
  
$x^{|n|} = x \cdot (x+1)\cdot (x+2)\cdots (x+n-1)$ - rising factorial
  
$x^{(n)} =x\cdot (x-1) \cdot (x-2) \cdots (x-n+1)$ - falling factorial.
  
Substituting a=1 and b=0 in (i) and (ii) above , we get that
  
$\Delta x^{(n)} = n\cdot x^{(n-1)}$ , $\Delta^n x^{(n)} = n!$ and $\displaystyle{\Delta \frac{1}{x^{|n|}} = - \frac{n}{x^{|n+1|}}}$.
  
Summary:

<figure>
  <img class="alignnone size-full wp-image-11204" src="https://gaurish4math.files.wordpress.com/2018/06/capture7.png" alt="Capture7" width="1021" height="262" /> 
  <figcaption>Richardson, C. H. <i>An introduction to the calculus of finite differences.</i> pp. 10.</figcaption>
</figure>

Due to the fact that $x^{(n)}$ plays in the calculus of finite differences a role similar to that played by $x^n$ in the infinitesimal calculus, for many purposes in finite differences it is advisable to express a given polynomial in a series of factorials. A method of accomplishing this is contained in <span style="text-decoration: underline;">Newton's Theorem</span>.

<figure>
  <img class="size-full wp-image-11205 aligncenter" src="https://gaurish4math.files.wordpress.com/2018/06/capture8.png" alt="Capture8" width="718" height="425" />
  <figcaption>Richardson, C. H. <i>An introduction to the calculus of finite differences.</i> pp. 10.</figcaption>
</figure>

Since these differences and $U_x$ are identities, they are true for all values of x, and consequently must hold for x = 0. Setting x = 0 in the given function and the differences, we have the required values for all $a_i$ and theorem is proved.
