---
layout: post
title: Power of Quadratics
abstract: Here is a very didactic algebra exercise I found that reveals a very instructive solution. I encourage you to take the time to explore and analyze the solutions carefully, because I feel like there is a meaningful lesson to be learnt here about the importance of context, background and exploration.
---

I saw a problem similar to the one I am about to present pass through my Twitter feed some time ago but unfortunately, I remember neither the author nor the exact nature of the equation involved. However, knowing the essence of its solution I managed to reverse-engineer a new problem that will hopefully have the same effect on the solver as the original problem had on me.

### The problem

Find all real values of $$x$$ that satisfy the equation
\begin{equation}
    (x^2-7x+11)^{(x^2-18x+77)}=1\text{.}
\end{equation}

*Scroll for solution (Spoilers!)*

<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>

### The solution

We first notice that we have an equation of the form $$A^B=1$$, where $$A$$ and $$B$$ are real numbers. Without worrying about the specific expressions contained in $$A$$ and $$B$$, let us first consider the different possibilities to solve this simple equation. This part of the solution is arguably the most insightful part because it requires care and an eye for detail.

So, what are the solutions for $$A$$ and $$B$$ ? 

1. $$B=0$$. We know that any number to the zeroth power is equal to one. Or should I say, *almost* any number. The subtlety here is that $$0^0$$ is undefined, so this solution only works if $$A\neq 0$$. This is something that needs to be verified for any solution we find to $$B=0$$.

2. $$A=1$$. This is a solution without exception. One raised to any power is still one.

3. $$A=-1$$. This is the solution that many people (including myself) miss at first sight. Careful consideration reveals that this is indeed a solution if $$B$$ is an even integer, since $$-1$$ raised to an even power is indeed one.

After some reflection, we come to the conclusion that any solution to $$A^B=1$$ must fall into (at least) one of the above three categories. An important constraint in this argument is that $$A$$ and $$B$$ are both real. Indeed, if $$A$$ or $$B$$ are allowed to be arbitrary complex numbers, then there are many more solutions and classifying them is no longer a trivial task.

Now, let us consider each of the above cases substituting in the expressions with $$x$$, i.e. $$A=x^2-7x+11$$ and $$B=x^2-18x+77$$.

1. $$B=0$$. This is equivalent to the quadratic equation $$x^2-18x+77=0$$ which can be factorized as $$(x-7)(x-11)=0$$ and therefore yields two candidates $$x=7$$ and $$x=11$$. A quick but important check verifies that $$A\neq 0$$ for either of these values, so they are indeed solutions of the problem.

2. $$A=1$$. This is equivalent to the quadratic equation $$x^2-7x+11=1$$, or $$x^2-7x+10=0$$ which can be factorized as $$(x-2)(x-5)=0$$. This directly yields two further solutions $$x=2$$ and $$x=5$$.

3. $$A=-1$$. This is equivalent to the quadratic equation $$x^2-7x+11=-1$$, or $$x^2-7x+12=0$$ which can be factorized as $$(x-3)(x-4)=0$$. This gives us two candidates $$x=3$$ and $$x=4$$, but they are not verified solutions until we check that $$B$$ is even for these cases. A simple calculation finds $$B=32$$ for $$x=3$$, so this is indeed a solution. For $$x=4$$, we obtain $$B=27$$ which is odd. Therefore, $$x=4$$ is in fact not a true solution to the problem! 

The full set of solutions is therefore $$x=2,3,5,7,11$$, or the first five prime numbers. Pretty cool, no?

In all seriousness, this problem illustrates that the underlying conditions and assumptions behind an equation or solution are just as important as the solution itself. This is a point that can be extrapolated to transcend mathematics or even the natural sciences: In order to understand and apply any law or relation correctly, it is fundamental not only to understand the law itself, but also to understand the context in which it is valid.