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
$$ \mid \phi \rangle  =  \alpha \mid 0 \rangle + \beta  \mid 1 \rangle $$, with $$ \mid \alpha \mid ^2 + \mid \beta \mid ^2 = 1 $$ (normalization)
where $$ \mid 0 \rangle $$  and $$ \mid 1 \rangle $$ are just two dimensional base vectors with<>
$$ \mid 0 \rangle = \begin{pmatrix} 1\\ 0 \end{pmatrix} $$ and $$ \mid 1 \rangle = \begin{pmatrix} 0\\ 1 \end{pmatrix} $$ , $$\mid 0 \rangle, \mid 1 \rangle \in \mathbb{C}^2 $$
You will see later on that the ket notation $$ \mid \cdot \rangle $$ is very useful.

In general the amplitudes $$ \alpha $$ and $$ \beta $$ cannot be measured directly, instead, one will get the result 
0, with probability $$ \mid \alpha \mid ^2 $$
1, with probability $$ \mid \beta \mid ^2 $$
Indirectly one can measure $$ \mid \alpha \mid ^2 $$ and $$ \mid \beta \mid ^2 $$ via repeating an experiment many times (trials/shots)
and after that examining the statistical outcomes.

In practice, a qubit can be different things:
    -two different polarizations of a photon
    -alignment of a nucler electron spin
    -ground state or excited state of an atom



*References:*
*[^1]:Download Julia: julialang.org*
