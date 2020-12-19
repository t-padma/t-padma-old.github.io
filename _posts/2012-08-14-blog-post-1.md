---
title: 'Enclosing closed curves in squares'
date: 2018-06-01
permalink: /posts/2018/06/enclosing-closed-curves-in-squares/
tags:
  - algebraic topology
  - closed-curve
  - combinatorial topology
  - continuity
  - continuous functions
  - difference
  - intermediate value theorem
  - length
  - real analysis
  - real line
  - square
  - topology
---
Let's look at the following innocent looking question:

<blockquote>
<p>Is it possible to circumscribe a square about every closed curve?</p>
</blockquote>

The answer is YES! I found an unexpected and interesting proof in the book<a href="https://books.google.co.in/books?id=CfjCuh3OvioC&amp;printsec=frontcover#v=onepage&amp;q&amp;f=false" target="_blank" rel="noopener"> "Intuitive Combinatorial Topology " by V.G. Boltyanskii and V.A. Efremovich</a> . Let's now look at the outline of proof for our claim:

1. Let any closed curve<strong> K</strong> be given. Draw any line <strong>l</strong> and the line <strong>l' </strong>such that line <strong>l'</strong> is parallel to<strong> l</strong> as shown in the fig 1.

<img class=" size-full wp-image-11180 aligncenter" src="https://gaurish4math.files.wordpress.com/2018/06/capture11.png" alt="capture11" width="307" height="381" />

 2. Move the lines <strong>l</strong> and <strong>l'</strong> closer to <strong>K</strong> till they just touch the curve <strong>K</strong> as shown in fig 2. Let the new lines be line <strong>m</strong> and line <strong>m'</strong>. Call these lines as the support lines of curve <strong>K</strong> with respect to line <strong>l</strong>.

<img class=" size-full wp-image-11181 aligncenter" src="https://gaurish4math.files.wordpress.com/2018/06/capture21.png" alt="capture21" width="306" height="395" />

 3. Draw a line<strong> l*</strong> perpendicular to<strong> l</strong> and the line <strong>(l*)'</strong> parallel to <strong>l*</strong> . Draw support lines with respect to line <strong>l*</strong> to the curve <strong>K</strong> as shown in the fig 3. Let the rectangle formed be ABCD .

<img class=" size-full wp-image-11182 aligncenter" src="https://gaurish4math.files.wordpress.com/2018/06/capture31.png" alt="capture31.png" width="456" height="393" />

 4. The rectangle corresponding to a line will become square when AB and AD are equal . Let the length of line parallel to<strong> l</strong> (which is AB)  be $h_1(\mathbf{l})$ and line perpendicular to <strong>l</strong> (which is AD) be $h_2(\mathbf{l})$. For a given line <strong>n</strong>, define a real valued function $f(\mathbf{n}) = h_1(\mathbf{n})-h_2(\mathbf{n})$ on the set of lines lying outside the curve <strong>K </strong>.  Now rotate the line <strong>l</strong> in an anti-clockwise direction till <strong>l</strong> coincides with <strong>l'</strong>. The rectangle corresponding to<strong> l*</strong> will also be ABCD (same as that with respect to <strong>l</strong>). When <strong>l</strong> coincides with <strong>l'</strong>, we can say that  $AB = h_2(\mathbf{l^{*}})$ and $AD = h_1(\mathbf{l^{*}})$.

<img class=" size-full wp-image-11183 aligncenter" src="https://gaurish4math.files.wordpress.com/2018/06/capture41.png" alt="capture41" width="475" height="402" />

 5. We can see that when the line is <strong>l</strong>, $f(\mathbf{l}) = h_1(\mathbf{l})-h_2(\mathbf{l})$. When we rotate <strong>l</strong> in an anti-clockwise direction the value of the function f changes continuously i.e. f is a continuous function (<em>I do not know how to "prove" this is a continuous function but it's intuitively clear to me; if you can have a proof please mention it in the comments</em>). When <strong>l</strong> coincides with <strong>l'</strong> the value of $f(\mathbf{l^*}) = h_1(\mathbf{l^*})-h_2(\mathbf{l^*})$. Since $h_1(\mathbf{l^*}) = h_2(\mathbf{l})$ and $h_2(\mathbf{l^*}) = h_1(\mathbf{l})$. Hence $f(\mathbf{l^*}) = -(h_1(\mathbf{l}) - h_2(\mathbf{l}))$. So f is a continuous function which changes sign when line is moved from <strong>l</strong> to <strong>l'</strong>. Since f is a continuous function, using the<a href="https://en.wikipedia.org/wiki/Intermediate_value_theorem#Generalizations" target="_blank" rel="noopener"> generalization of intermediate value theorem </a>we can show that there exists a line <strong>p</strong> between <strong>l</strong> and <strong>l*</strong> such that f(<strong>p</strong>) = 0 i.e. AB = AD.  So the rectangle corresponding to line <strong>p</strong> will be a square.

Hence every curve <strong>K</strong> can be circumscribed by a square.
