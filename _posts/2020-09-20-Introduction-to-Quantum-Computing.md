---
title: Introduction-to-Quantum-Computing
layout: post
---



# Hello and Welcome to another article! #

First, let us take a look to the math needed in this subject.
The actual math consists mainly of basic linear algebra.
A general knowledge of quantum phisics is a great advantage too.
As for me, I will use Julialang in the code examples, wich looks like Python, feels like Lisp, and runs like C.[^1]


In quantum computation we use, instead of the regular bits wich have either the state 1 or 0, so called "qubits", wich are the superposition of the sate 1 and 0. A quantum state $$ \mid \phi \rangle $$ is described as 
$$ \mid \phi \rangle  =  \alpha \mid 0 \rangle + \beta  \mid 1 \rangle $$
where $$ \mid 0 \rangle $$  and $$ \mid 1 \rangle $$ are just two dimensional base vectors with
$$ \mid 0 \rangle = \begin{pmatrix} 1\\ 0 \end{pmatrix} $$ and $$ \mid 1 \rangle = \begin{pmatrix} 0\\ 1 \end{pmatrix} $$ , $$\mid 0 \rangle, \mid 1 \rangle \in \mathbb{C}^2 $$
You will see later on that the ket notation $$ \mid \cdot \rangle $$ is very useful.  


*References:*
*[^1]:Download Julia: julialang.org*
