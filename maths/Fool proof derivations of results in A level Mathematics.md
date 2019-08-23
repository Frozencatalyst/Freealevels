# Fool proof derivations of results in A level Mathematics

[TOC]

### Fundamental definitions

- Sets of numbers: $$\N = \{1,2,3,...\}$$, $$\Z = \{...,-1,0,1,...\}$$,$$\Q = \{\tfrac{p}{q} | p,q \in \Z, q \neq 0 \}$$.
- The set of real numbers, $$\R$$, includes rational and irrational numbers; all quantities with a measurable length.
- Basic operations and their properties are assumed (multiplication, addition and their inverses)

Further definitions will be defined throughout.

### Algebra

#### 1. Quadratics

- Definition 1P: A quadratic is an equation which can be represented in the form: $$ax^2 + bx + c = 0$$ where $a,b,c \in \R$ and $a \neq 0$.

We are able to use elementary algebra to rearrange and solve for $$x$$; giving us the quadratic formula via completing the square:
$$
\begin{align}
ax^2 + bx + c &= a(\dfrac{ax^2+bx}{a}) + c \\
&=a(x^2 + \dfrac{b}{a}x) + c
\end{align}
$$
We can formulate a "perfect square", $$(a + b)^2$$ by noticing that: $$(x + \dfrac{b}{a})^2 = x^2 + 2(\dfrac{b}{a})x + (\dfrac{b}{a})^2$$:
$$
a(x^2 + \dfrac{b}{a}x) + c = a(x + \dfrac{b}{2a})^2 - \dfrac{b^2}{4a} + c \; \; \; \; \text{  (1): Completed square quadratic form.} \\
\dfrac{b^2}{4a^2} - \dfrac{c}{a} = (x + \dfrac{b}{2a})^2 \\
-\dfrac{-b}{2a} \pm \dfrac{\sqrt{b^2 - 4ac}}{2a} = x \; \; \; \; \text{  (2): General quadratic formula.}
$$
If we consider $\alpha, \beta$ as the first and second roots of a quadratic and consider that we can divide through any quadratic by the leading coefficient to end up with: $$x + bx^2 + c$$ as the general form of a quadratic:
$$
\begin{align}
\dfrac{a(x-\alpha)(x - \beta)}{a} &= \dfrac{ax^2 + bx + c}{a} \\
x^2 - (\alpha + \beta)x + \alpha \beta &= x^2 + \dfrac{b}{a}x + \dfrac{c}{a}
\end{align}
$$
We can "equate coefficients" to derive the sum rule of roots and the product rule:
$$
-(\alpha + \beta) = \dfrac{b}{a} \; \text{or} \; \alpha + \beta = -\dfrac{b}{a} \; \; \; (3) \text{ Sum of roots} \\
\alpha \beta = \dfrac{c}{a} \; \; \; (4)  \text{ Product of roots}
$$

#### 2. Factor and remainder theorem.

- Definition 2P: For any real number, $b = qa + r$, where b is the dividend, a the divisor, q the quotient and r the remainder: $$ 0 \leq r < |a| $$ (Euclid's division)

Using euclid's division we  can prove the factor and then remainder theorem:



