## <u>STEPping maths up a notch</u>

[TOC]

<u>STEP problems with worked solutions and commentary</u>

This a compilation of working through STEP problems. As much of the initial working remains intact as possible and explanations our as thorough as possible. Questions are from: http://www.colmanweb.co.uk/Assets/PDF/advanced-problems-mathematics.pdf

#### Starting out

From 2000 paper 1:

- Let $$f(x) = ax - \dfrac{x^3}{1+x^2}$$, where $$a$$ is a constant. Show that when $$a \geq \dfrac{9}{8}$$, for all values of $x$, $$f'(x) \geq 0$$

First thoughts:

1. We are going to need to differentiate; use of the [quotient rule](http://www.mathcentre.ac.uk/resources/uploaded/mc-ty-quotient-2009-1.pdf) seems the best avenue here; chain rule seems overkill.
2. We need to be aware of the general shape of the derivative, the easiest way will be to check whether $$f(x)$$ is [even/odd function](https://en.wikipedia.org/wiki/Even_and_odd_functions) which will imply the derivative being the opposite.
3. To determine whether the function will intercept the y-axis we need to find the stationary point(s) and determine their nature; for a quadratic we can easily do this via completing the square or using the discriminant - hopefully we can get away with this.

Solving the problem:

Let's begin by testing the evenness of the function: 
$$
f(-x) = -ax + \dfrac{x^3}{1 + x^2} \therefore -f(-x) = f(x)
$$
We now see that $$f(x)$$ is odd which means $$f'(x)$$ is even. This is good as it means the 2 tails will go one direction; and as such may not intercept the x-axis. Now let's differentiate the function:
$$
f'(x) = a - \dfrac{d}{dx}(\dfrac{x^3}{1+x^2}) = a - \dfrac{(1+x^2)3x^2- x^2(2x)}{(1+x^2)^2}
$$
The denominator here will always be positive; so we should make this common and then concern ourselves with the nature of the numerator. Then we should use algebraic manipulation to get it into a form were comfortable with (ideally quadratic):
$$
\begin{align}
\dfrac{a(1+x^2)^2 - (3x^2(1+x^2) - 2x(x^3))}{(1+x^2)^2} &= \dfrac{a(1 + 2x^2 + x^4) - (3x^2 + x^4)}{''} \\
&= \dfrac{a + (2a-3)x^2 + (a - 1)x^4}{''} \; \; \; (1)
\end{align}
$$
NB, the ditto '' is used to represent no change; an irrelevancy to the current evaluation (yet it is still there!).

Now we have a quadratic; let us complete the square to find the minimum point (and to see whether this satisfies the original question):
$$
Au^2 + Bu + C, u = x^2 \\
A(u + \dfrac{B}{2A})^2 - \dfrac{B^2}{4A} + C \\
A = a - 1, B = 2a - 3, C = a
$$

$$
\begin{align}
(a-1)(x^2 + \dfrac{2a - 3}{2(a-1)})^2 - \dfrac{(2a-3)^2}{4(a-1)} + a
\end{align}
$$

We can see if we plug $$9/8$$ the first term (in brackets) is positive so we need to find whether this is the case for the second term by some algebraic manipulation:
$$
\dfrac{4a(a - 1) - (2a - 3)^2}{4(a - 1)} = \dfrac{8a - 9}{''}
$$
As we can see we require $$ a \geq \dfrac{9}{8}$$ for this term to be positive; demonstrating what was asked of us in the question. QED ("thus it has been demonstrated"). However we are not completely done as we should now check the conditions for each variable in the completed square to be positive. 

Remarks:

- A simpler solution would have been, after reaching (1), to have substituted the inequality,  $$a \geq \dfrac{9}{8}$$, into a and solved; making completing the square an unneccesary procedure:

$$
a \geq \dfrac{9}{8} \; f'(x) = \dfrac{\dfrac{1}{8}(x^4 - 6x^2 + 9)}{(1 + x^2)^2}
$$

- And finishing by rewriting the top as a perfect square, $(a - b)^2 = a^2 - 2ab + b^2$, $a$ would be $x^2$ and $b$ must be $-3$: 

$$
f'(x) = \dfrac{(x^2 - 3)^2}{8(1+x^2)^2} \geq 0
$$

From 1999 paper 1:

- The $$n$$ positive numbers $$x_1, x_2, ..., x_n$$, where $$n \geq 3$$ satisfy:
  $$
  x_1 = 1 + \dfrac{1}{x_2}, x_{n-1} = 1 + \dfrac{1}{x_n}
  $$



- And also that:

$$
x_n = 1 + \dfrac{1}{x_1}
$$

- Show that:
  - $$x_1,x_2,...,x_n > 1$$ (i)
  - $x_1 - x_2 = \dfrac{x_2 - x_3}{x_2 x_3}$ (ii)
  - $$x_1 = x_2 = ... = x_n$$ (iii)

First thoughts:

- The easiest way to attempt (i) is to assume (iii) to be true, then going back to (iii) to solve the final part.
- (ii) seems the easiest as we can simply use the identities given in the question to solve it.

Solving the problem:

For (i) Assume (iii) to be true which means:
$$
x_1 = x = 1 + \dfrac{1}{x}
$$
I instantly recognise this as the quadratic of the golden ratio; $$ x = \dfrac{2 + \sqrt{5}}{2}$$; we know that $$x_n$$ are positive numbers so we removed $$- \sqrt{5}$$ as the other solution. This shows that $$x_1, x_2, x_3... > 1 $$ if (iii) is true.

For (ii):
$$
x_1 - x_2 = (1 + \dfrac{1}{x_2}) - (1 + \dfrac{1}{x_3}) = \dfrac{1}{x_2} - \dfrac{1}{x_3} = \dfrac{x_3 - x_2}{x_2x_3}
$$


