# Numerical Evaluation of a Limit

Perform all your calculations for this problem in double precision.

Consider the following limit:

$$\lim_{x \to 0} \frac{e^{x} - 1}{x}$$

Using L'Hopital's rule, it is straigtforward to prove that the value of this limit is `1`.

Write C++ code that numerically estimates the value of the above limit, by evaluating $\frac{e^{x} - 1}{x}$ for several values of `x`.
In particular, use values of $x = 10^{-5}$, $10^{-6}$, $10^{-7}$, $10^{-8}$, $10^{-9}$, $10^{-10}$, $10^{-11}$, $10^{-12}$, $10^{-13}$, $10^{-14}$, and $10^{-15}$.
Report your results at the end of this `README.md` file.

Now, we'll try a mathematically equivalent (but algorithmically different) approach to the same problem.
We'll define $y = e^{x}$.
We can then say that 

$$\lim_{x \to 0} \frac{e^{x} - 1}{x} = \lim_{y \to 1} \frac{y - 1}{\ln{(y)}}$$

Write code that computes $y$ for the same set of values of $x$ as before ($x = 10^{-5}$, $10^{-6}$, $10^{-7}$, $10^{-8}$, $10^{-9}$, $10^{-10}$, $10^{-11}$, $10^{-12}$, $10^{-13}$, $10^{-14}$, and $10^{-15}$).
Then evaluate $\frac{y - 1}{\ln{(y)}}$ for the resulting values of $y$.
Remember that the `log` function from `math.h` computes the natural log of its argument.
Report your results at the end of this `README.md` file.

At the end of this `README.md` file, explain your observations *in detail*, including the *specific reasons* for any differences in numerical stability.

## Answer
