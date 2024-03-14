---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Vectors and their Properties

## What are Vectors?

In mathematics, and in its use, we often quantify amounts/states such as mass, time, force, economic conditions, circuit voltages, and points in space. However, only some of these quantities can be expressed using a single number (i.e. mass & time). To represent more complex _multi-component_ quantities we must use multiple numbers. We can do this using vectors.

Vectors can represent lots of different quantities; here are a couple.

```{tab} Points in 2D Space
$$
  \vec{v} = \bmatrix x \\ y \ematrix
$$
When $x$ and $y$ are real numbers (i.e. $x,y \in \R$), the vector $\vec{v}$ can represent any point in 2D space. This is possible because we can assign every point in 2D space a unique pair of *coordinates* $x$ and $y$.
+++
```

```{tab} Another example...
more stuff!
```

```{prf:definition} Linear Equation
:label: linear-equation
A **linear equation** is an equation with finite terms of the form

$$
  a_1 x_1 + a_2 + \ldots + a_n x_b = b
$$

where $x_1, x_2, \ldots, x_n$ are variables (i.e. unknowns), $a_1, a_2, \ldots, a_n$  and $b$ are scalars (i.e. coefficients of the equation), and $n$ is a {abbr}`natural number ({1, 2, 3, ...})` (i.e. # of variables).

More simply, a linear equation is the equation formed by taking a degree-one multi-variate polynomial and setting it equal to 0.
```

````{prf:example} Some Linear Equations
Determine which of the following equations are *linear*.

$$
  3 x_1 + 4 x_2 &= -2 x_1\\
  (2 + x_1) x_2 &= 6\\
  \sqrt{5} x_1 + 4 x_2 &= 0\\
  5 \sqrt{x_1} + 4 x_2 &= 0
$$

```{toggle}
1. The first equation is linear since it can be rewritten as $5 x_1 + 4 x_2 = 0$.
2. The second equation is **not** linear as we can re-express it as $2 x_2 + \boxed{x_1 x_2} = 6$. The term $x_1 x_2$ has degree 2, so the degree of the equation is at least two. Therefore, the second equation is not a linear.
3. The third equation is linear as we can have $a_1 = \sqrt{5}$ and $a_2 = 4$ thus satisfying {prf:ref}`linear-equation`.
4. The fourth equation is **not** a linear equation as it is not a polynomial since $\sqrt{x_1}$ is not a variable with a non-negative integer power.
```

````
