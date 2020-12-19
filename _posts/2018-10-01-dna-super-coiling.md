---
title: 'DNA super-coiling'
date: 2018-10-01
permalink: /posts/2018/10/dna-super-coiling/
tags:
  - topology
  - knot theory
  - dna
  - biology
---

DNA super-coiling is said to occur when the DNA strand experiences strain which is either due to over-winding or under-winding of DNA. DNA super-coiling is important in a number of biological processes. In this post we would like to use a branch of topology to explain super-coiling. Before going to the topology part, we need to know some basics about the structure of DNA. I have written this blog by following the book <a href="https://bookstore.ams.org/KNOT" target="_blank" rel="noopener">"The knot book" by Colin Adams</a>.

## Structure of DNA
It is well known that deoxy-ribonucleic acid or DNA is a double helix that contains the instructions an organism needs to develop, live and reproduce. DNA is formed by pairs of long molecular strands that are bonded together by ladder rungs. This structure spirals around itself to get the double helix structure.

![zero](https://gaurish4math.files.wordpress.com/2018/09/pic1.jpg)

The molecular strands are made of alternating sugars and phosphates. Each sugar is bonded to one of four bases - Adenine(A) , Thyamine(T) , Cytosine(C) , Guanine(G). The rungs are formed by hydrogen bonds between bases. Note that hydrogen bonds are always formed between "A", "T" and "G", "C". The sequence of A's , T's , G's , C's as we run down one of the strands is the genetic code (which gives a blueprint for life).

The sugar molecule of the strand is deoxy-ribose sugar molecule. The carbons of each sugar molecule can be numbered due to which every sugar has a 5' end and a 3' end as shown below.

![first](https://gaurish4math.files.wordpress.com/2018/09/pic3.jpg)

![second](https://gaurish4math.files.wordpress.com/2018/09/pic4.jpg)


DNA has anti parallel strands i.e. as we go down, if we run through 5' carbon to 3' carbon on one strand then we will run through  5' carbon to 3' carbon on the other strand only if we move upward. A single stranded DNA by convention has an orientation,  we should start at 5' end and move towards 3' end. On the other hand a linear duplex DNA has no orientation since a 3' site on one strand is opposite to 5' site on the other.

## Modelling DNA
DNA can be modelled in two ways. We can look at DNA either as a ribbon or as a curve. If we represent the DNA by the axis of the DNA, we get a curve in three dimensions. Other way to look at DNA is by considering it as a ribbon whose ends represent the two molecular strands of DNA.

<figure class="image">
  <img src="https://gaurish4math.files.wordpress.com/2018/09/dna1.jpg" alt="a">
  <figcaption>DNA</figcaption>
</figure>

<figure class="image">
  <img src="https://gaurish4math.files.wordpress.com/2018/09/dna2.jpg" alt="b">
  <figcaption>DNA as a curve</figcaption>
</figure>

<figure class="image">
  <img src="https://gaurish4math.files.wordpress.com/2018/09/dna3.jpg" alt="c">
  <figcaption>DNA as a ribbon</figcaption>
</figure>


As it can be seen in the picture below, for the duplex DNA to be circular, we need to have even number of half twists when DNA is laid flat on plane . Since there must be two distinct edges(two molecular strands) for the DNA modelled as a ribbon, hence cyclic duplex DNA cannot form a mobius strip( Since a mobius strip has only one edge).

![third](https://gaurish4math.files.wordpress.com/2018/09/pic5.jpg)


## Why does DNA super-coiling happen? 

In order to answer the above question, we will have to know some very basic knot theory definitions.

A mathematical <strong>knot </strong>is just a knotted loop of string such that the string has no thickness and its cross section is assumed to be a single point. Note that a knot should not have free ends. It has to be closed. All the knots that we obtain by deforming a particular knot, say K , will be considered equivalent to K if they have been formed by continuous deformation not involving cutting of knot.

<figure>
  <img class=" size-full wp-image-11247 aligncenter" src="https://gaurish4math.files.wordpress.com/2018/10/knot.jpg" alt="knot" width="597" height="193" />
  <figcaption>Adams,C. <i>The Knot Book</i></figcaption>
</figure>


Above picture shows three equivalent knots. From above example we realize that the same knot can have different pictures. Each such picture is called a <strong>projection</strong> for the knot. The places where a knot crosses itself in the picture is called a <strong>crossing</strong> of the projection. An example is given below to understand crossings and projections better.


<figure>
  <img class=" size-full wp-image-11248 aligncenter" src="https://gaurish4math.files.wordpress.com/2018/10/projection.jpg" alt="projection" width="586" height="187" />
  <figcaption>Adams,C. <i>The Knot Book</i></figcaption>
</figure>


While a knotted loop is called a knot, a set of such knotted loops tangled together is called a <strong>link</strong> . Just like in case of knots, two links are called equivalent if one link can be formed from another through continuous deformation which doesn't involving cutting. Example of a link is the Whitehead link.

<figure>
  <img class=" size-full wp-image-11249 aligncenter" src="https://gaurish4math.files.wordpress.com/2018/10/white.jpg" alt="white" width="388" height="148" />
  <figcaption>Adams,C. <i>The Knot Book</i></figcaption>
</figure>


We can see in the above picture that the Whitehead link is made of two loops knotted with each other. So we say that the Whitehead link has two <strong>components.</strong> Hence we can define a knot to be a link with only one component.

Linking number which I will define for a link is a topological invariant i.e. it is invariant under deformations which don't involve cutting

Now a circular duplex DNA can be considered as a link with two components. (Two components are the two strands ).

Suppose we have a ribbon (DNA) in space. Assume that this ribbon is rigidly fixed in space. Twist (Tw) and Writhe (Wr) of the ribbon are invarients which depend on the particular placement of ribbon in space. Moving the ribbon can change the twist and writhe of the ribbon.

<!--- **Twist (Tw):** --->

<!--- Twist of the ribbon measures how much the ribbon twists around its axis. Given a ribbon, twist is calculated in the following way. --->
