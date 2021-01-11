---
title: Introduction to calculus of variations
layout: post

---
A brief Introduction to the Euler-Lagrange equations.

...

Definition: Let\\(\mathrm{V}\\) be a \\(\mathbb{K}\\) Vectorspace. 
A mapping \\(\mathcal{F}\\) : \\(\mathrm{V} \rightarrow \mathbb{K}\\) is called a "Functional". In the following let \\(\mathbb{K}=\mathbb{R}\\).

Let's see an example:  
$$\mathrm{V} =  \{ x  \in   \mathscr{C}^1([ 0, 1])| \text{ x(0) = x(1) = 0} \}$$
$$\mathcal{F} (x) = \int\limits_0^1 \sqrt{1+\dot{x}^2} \mathrm{d}x$$

As you can see \\(\mathcal{F}\\) is a function of a function. You will see later on some more physical examples ("Action").

The basic problem of calculus of variations is to minimize a function, if necessary under constraints. In order that \\(\mathcal{F}\\)can have a minimum at \\(x \epsilon \mathrm{V}\\) in \\(\mathrm{U} \subseteq \mathrm{V}\\), it has to fulfill (if \\(\mathcal{F} \epsilon \mathscr{C}^1\\) ) : 

$$\frac{\mathrm d}{\mathrm d x }\mathcal{F}( x + \varepsilon  h ) |_{\varepsilon=0}  = F'(x)h = 0$$

\
\\(\forall h \varepsilon \mathcal{F}\\) : such that h vanishes at the bounderies, for wich \\(x +\varepsilon h \in \mathrm{U}\\), for sufficient small \\(\varepsilon \neq 0\\). 

 This means that x has to be a stationary point. The most "common" and widely seen class of functionals are of the form:

$$\mathrm{F}(x) = \int\limits_{t_1}^{t_2} \mathcal{L}\big(t, x(t), \dot{x}(t)\big) \mathrm{d} t$$

$$\mathcal{L} \in \mathscr{C}^2 ([t_1, t_2] \times \mathbb{R}^m \times \mathbb{R}^m, \mathbb{R}) $$ is called "Lagrange-function" or lagrangian, and $$ x : [0, 1] \rightarrow \mathbb{R}^m $$ is out of a suitable $$ \mathscr{C}^1 $$-functionspace $$ \mathrm{V} $$ .

Now we'll take a look at what happens if m=1 and 
\\(\mathrm{V} = { x \in  \mathscr{C}^2 ([ t_1, t_2])|\text{ } x(t_1) = x(t_2) = 0 }\\).

Suppose we have a stationary point at \\(x \in \mathrm{V}\\), this means for all \\( \in \mathrm{V}\\)that\: 

 $$ 0 = \frac{\mathrm d}{\mathrm d \varepsilon } \mathcal{F} ( x + \varepsilon  h ) |_{\varepsilon = 0} = \frac{\mathrm d}{\mathrm d \varepsilon } \int\limits_{t_1}^{t_2} \mathcal{L} \big( t, x(t) + \varepsilon h(t) , \dot{x} (t) + \varepsilon \dot{h} (t) \big) |_{ \varepsilon = 0} \mathrm{d} t$$ 
 \
 
 After pulling \\(\frac{\mathrm d}{\mathrm d \varepsilon }\\) inside the Integral it follows with the chain rule:\

 $$0 =\int\limits_{t_1}^{t_2}\Big[ \frac{\partial\mathcal{L}}{\partial x}h +\frac{\partial\mathcal{L}}{\partial \dot{x}}\dot{h} \Big] \mathrm{d}t=^1 \int\limits_{t_1}^{t_2}\frac{\partial\mathcal{L}}{\partial x}h\mathrm{d}t+\frac{\partial\mathcal{L}}{\partial\dot{x}}h\Big|_{t_1}^{t_2} -\int\limits_{t_1}^{t_2}\frac{d}{dt}\frac{\partial\mathcal{L}}{\partial\dot{x}}hdt=^2 \int\limits_{t_1}^{t_2}h\Big[\frac{\partial\mathcal{L}}{\partial x}-\frac{d}{dt}\frac{\partial\mathcal{L}}{\partial\dot{x}}\Big]dt$$
 Where  at [1] we integrated by parts. Then at [2] we used that h vanishes at the boundaries.
 What we got are is called an Euler-Lagrange Equation:

 $$\frac{\partial\mathcal{L}}{\partial x}-\frac{d}{dt}\frac{\partial\mathcal{L}}{\partial\dot{x}}=0$$

This equation provides the solution for our extrem value problem.




