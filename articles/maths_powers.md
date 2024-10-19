# Aren't powers just repeated multiplication?

In mathematics, a core approach to developing our ideas is that of _extending_ definitions. Let's explore this by taking a look at the concept of _powers_, which you should be familiar with from high school. Back then, you probably learnt that the definition of a power is just repeated multiplication:

$$ 3^{4} = 3 \times 3 \times 3 \times 3 $$

Often when we start with a definition like this, we notice that it produces other properties that are always true. To demonstrate this, let's take a look at what happens when you take two different powers of a number and multiply them together:

$$ 2^{3} \times 2^{4} = 2 \times 2 \times 2 \times 2 \times 2 \times 2 \times 2 = 2^{7} $$

You can see that $2^{3}\times2^{4}$ is just multiplying $2$ by itself 3 times, and then again by another 4 times, so $2^{3}\times2^{4}=2^{3+4}={2^7}$. We can write this more generally as:

$$ n^{a} \times n^{b} = n^{a+b} $$

What's important to note here is not just that this relationship is derived from the original definition of repeated multiplication, but that it is also _always_ true, no matter what values of $n$, $a$ and $b$ we choose. But if it's _always_ true, then couldn't we also use it as a definition?

Before we answer that question, let's have a look at some patterns:

$$
\begin{equation}
\begin{aligned}
& 3^{6} = 729 \\
& 3^{5} = 243 \\
& 3^{4} = 81 \\
& 3^{3} = 27 \\
& 3^{2} = 9 \\
& 3^{1} = 3 \\
\end{aligned}
\end{equation}
$$

To get from $3^{6}$ to $3^{5}$, we simply divided by $3$. Then to get from $3^{5}$ to $3^{4}$, we again divided by $3$. And we could keep going with this pattern until we got down to $3^{1}=3$. But can we go any further? Each time, we divided by the _base_, $3$, and decreased the power by 1. What happens if we keep going?

$$
\begin{equation}
\begin{aligned}
& 3^{6} = 729 \\
& 3^{5} = 243 \\
& 3^{4} = 81 \\
& 3^{3} = 27 \\
& 3^{2} = 9 \\
& 3^{1} = 3 \\
& 3^{0} = 1 \\
& 3^{-1} = \frac{1}{3} \\
& 3^{-2} = \frac{1}{9} \\
& 3^{-3} = \frac{1}{27} \\
\end{aligned}
\end{equation}
$$

Continuing the pattern seems to give a somewhat reasonable answer, but raises some important questions:
- What does it mean to raise a number to the power of 0?
- What does it mean to raise a number to the power of a negative number?

To answer these, we need to go back and think about our original definition. We defined a power as repeated multiplication, and we can imagine such an idea in multiple ways.

For instance, the volume of a cube with side length 2 is $2\times2\times2=2^{3}=8$. <TODO: insert picture or gif of a cube broken into 8 pieces>. You can think of this by starting with (you could also start with a point and extend that into a line of length 2) a line of length 2, then extending it out to become a square with side length 2, that has $2\times2=4$ smaller squares, then extending that out to become a cube with side length 2. <TODO: insert gif with animation of this process (maybe learn manim?)>

You could also imagine a scenario where say, the population of rabbits tripled every year. If we started with just 3 rabbits, then in each year we would have the following populations:

$$
\begin{equation}
\begin{aligned}
& Year 1: 3 = 3^{1} \\
& Year 2: 9 = 3^{2} \\
& Year 3: 27 = 3^{3} \\
& Year 4: 81 = 3^{4} \\
& Year 5: 243 = 3^{5} \\
& Year 6: 729 = 3^{6} \\
\end{aligned}
\end{equation}
$$

There are endless other examples we could use, but the common thread between them is that they all rely on the idea that the next step of a pattern is to multiply by the same number over and over. In both of our examples, we actually could go backwards and start with the $0^{th}$ power. For the cube example, we could start with a single point, and then have it grow into a line, with two line segments. And for the rabbits, if we started with just 1 rabbit, then we would still be able to triple it to get to the next year's population of 3.

We can think of this idea algebraically too. Since 1 multiplied by any number is just that number, you could alternatively define a power as how many times you multiply 1 by some number.

TODO: insert equation here when i can be bothered

If you simply multiply 1 by a number 0 times, then you simply end up with 1. That matches the pattern we saw earlier, and still allows us to define powers as being repeated multiplication. So that gives us a clearly extended definition of powers that includes 0, but does it work for the negative numbers we saw in our pattern?


- TODO: talk about how multiplying negative times could be division
- TODO: talk about how extending definitions means examples and analogies might break down/not be general enough
- TODO: talk about how n^a+b makes this all a lot easier to work with
- TODO: talk about fractional powers/surds: n^1/2 * n^1/2 = n^1
- TODO: figure out equation numbers in latex
- TODO: figure fix formatting on year 1, year 2, year 3...

