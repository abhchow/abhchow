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