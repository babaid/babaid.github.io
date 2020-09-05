---
title: Introduction to calculus of variations
layout: post

---
Intro:

...

Definition: Let $$ \mathrm{V}$$ be a $$ \mathbb{K}  $$ Vectorspace. A mapping $$ \mathcal{F}$$ : $$ \mathrm{V} \rightarrow \mathbb{K} $$ is called a "Functional".  
In the following let $$ \mathbb{K}=\mathbb{R} $$.

Let's see an example:  
$$ \mathrm{V} = $$ { x $$ \epsilon $$ $$ \mathscr{C}^1(\[ 0, 1\])|x(0)= x(1) = 0} $$  
$$ \mathcal{F} (x) = \int\limits_0^1 \sqrt{1+\dot{x}^2}: \mathrm{d}x $$

As you can see $$ \mathcal{F} $$ is a function of a function. You will see later on some more physical examples ("Action").

The basic problem of calculus of variations is to minimize a function, if necessary under constaints. In order that $$ \mathcal{F} $$ can have a minimum at $$ x \epsilon \mathrm{V} $$ in $$ \mathrm{U} \subseteq \mathrm{V} $$, it has to fulfill (if $$ \mathcal{F} \epsilon \mathscr{C}^1$$ ) :\

$$ \frac{\mathrm d}{\mathrm d x } \left( \mathcal{F}( x + \epsilon * h ) |_\epsilon=0 $$