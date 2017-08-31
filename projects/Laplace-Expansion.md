---
layout: project
type: project
image: images/matrix.jpg
title: Laplace Expansion
permalink: projects/laplace
date: 2017
labels:
  - Matrices
  - Determinant
  - Linear Algebra
  - Laplace Expansion
summary: Explaining how the Laplace Expansion of a matrix works for anyone to understand and prove their equivalence to the standard definition of the determinant.
---

<img class="ui medium left floated image" title="Look, a matrix matrix!" src="../images/matrices.gif">

From MATH 311, the second project was to research Laplace expansions, a method for finding the determinant of a matrix, come to understand them, and be able to explain them to someone without any prior knowledge, including demonstrating its equivalence to the more standard formula for finding the determinant.  Though the paper goes into the explanation in more detail, Laplace expansions rewrite the standard definition of the determinant so that it is in terms of the determinants of a series of smaller sub-matrices and a series of coefficients.  The standard definition involves the sum of all possible permutations of a function, the Laplace definition allows the determinant to be found via recursion instead, creating numerous smaller problems.

While I held responsibility for the first draft of this project, Joshua and Jaren (as seen on the front page of the paper) were responsible for the formatting, proof-reading, corrections and revisions of the paper.  I was largely constructed responsible for constructing the proof and the multiple layers of kludgy set-up leading to proving the equivalence of the two methods of finding the determinant of a matrix.

There is frequently more than one way to accomplish a task, the trick is knowing what to use when.  When talking about large matrices, it can be hard to keep track of all the individual permutations as is required by the standard definition.  Laplace would require less code and be easier to adapt to any size matrix should one choose to automate the process.  On medium sized matrices, the Laplace method can allow one to create several smaller matrices to which a simple formula may be applied.  Longform equations work well for smaller matrices, but grow out of hand by the 4 by 4 size.

Paper: <a href="https://docs.google.com/document/d/1xei5mYIneCADmh33TDhonANqa1dTRRN7YIY5BDkuf1A/edit?usp=sharing"><i class="large File Word Outline icon"></i>Laplace</a>
