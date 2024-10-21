---
title: "stuff"
permalink: articles/maths_powers
layout: default
# layout: page
---

# Aren't powers just repeated multiplication?

## Part 1: An introduction
In mathematics, a core approach to developing our ideas is that of _extending_ definitions. Let's explore this by taking a look at the concept of _powers_, which you should be familiar with from high school. Back then, you probably learnt that the definition of a power is just repeated multiplication:

$$ 3^{4} = 3 \times 3 \times 3 \times 3 $$

Often when we start with a definition like this, we notice that it produces other properties that are always true. To demonstrate this, let's take a look at what happens when you take two different powers of a number and multiply them together:

$$ 2^{3} \times 2^{4} = 2 \times 2 \times 2 \times 2 \times 2 \times 2 \times 2 = 2^{7} $$

You can see that $2^{3}\times2^{4}$ is just multiplying $2$ by itself 3 times, and then again by another 4 times, so $2^{3}\times2^{4}=2^{3+4}={2^7}$. We can write this more generally as:

$$ n^{a} \times n^{b} = n^{a+b} $$

This is a much more convenient way to work with powers than writing out the repeated multiplication every time we come across them. Importantly, this relationship isn't just derived from the original definition of repeated multiplication, but it is also _always_ true, no matter what values of $n$, $a$ and $b$ we choose. But if it's _always_ true, then couldn't we also use it as a definition?

## Part 2: Extending the original definition
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

TODO: figure out how to underline stuff in latex so I can write a note that looks like |--------n times--------|

If you multiply 1 by a number 0 times, then you simply end up with 1. That matches the pattern we saw earlier, and still allows us to define powers as being repeated multiplication. So that gives us a clearly extended definition of powers that includes 0, but does it work for the negative numbers we saw in our pattern?

It doesn't really make sense to say that we multiplied a negative amount of times. But if negative numbers are the opposite of positive numbers, then maybe a negative power is the opposite of multiplying repeatedly - dividing repeatedly. 

$$
\begin{equation}
\begin{aligned}
& 3^{1} = 3 \\
& 3^{0} = 1 \\
& 3^{-1} = \frac{1}{3} \\
& 3^{-2} = \frac{1}{9} \\
& 3^{-3} = \frac{1}{27} \\
& 3^{-4} = \frac{1}{81} \\
& 3^{-5} = \frac{1}{243} \\
\end{aligned}
\end{equation}
$$

This is actually exactly what we did to create our pattern in the first place, we just kept on dividing by 3 to go backwards through the powers. So now we've extended our definition again, to say that a power is repeated multiplication for positive powers, and repeated division for negative powers.

## Part 3: A better definition
Can we extend the definition more? So far we've only defined how integer powers work. What about fractional powers? It doesn't make any sense to only multiply or divide _half_ a time. Can we come up with a definition that works for _all_ different numbers?

Well actually, we already did. Earlier, we noted the property 

$$ n^{a} \times n^{b} = n^{a+b} $$

Before we try to use this to further extend our definition, let's verify that it works as we expect for both negative and 0 powers. We'll start with showing that a number to the power of 0 should equal 1:

$$
\begin{equation}
\begin{aligned}
& 3^{5} \times 3^{0} = 3^{5+0} \\
& 3^{5} \times 3^{0} = 3^{5} \\
& 3^{5} \times 3^{0} = 3^{5} \times 1 \\
& 3^{0} = 1 \\
\end{aligned}
\end{equation}
$$

Now let's work on the negative powers. If we multiply a number by itself 5 times, but then divide it by itself 3 times, we should end up with that number multiplied by itself twice:

$$
\begin{equation}
\begin{aligned}
& 3^{5} \times 3^{-3} = 3^{5-3} \\
& 3^{5} \times 3^{-3} = 3^{2} \\
\end{aligned}
\end{equation}
$$

Notice that for both of these, we didn't need to use the idea of repeated multiplication or division to find these results. This is what makes it a great candidate for a new definition, because it does all of the same things, but lets us break free of the old and restrictive ideas.

We can actually do the same thing to see the relationship between positive, negative and 0 powers. If you multiply a number by itself 5 times, but then divide by itself 5 times, you should get right back to 1.

$$
\begin{equation}
\begin{aligned}
& 3^{5} \times 3^{-5} = 3^{5-5} \\
& 3^{5} \times 3^{-5} = 3^{0} \\
& 3^{5} \times 3^{-5} = 1 \\
\end{aligned}
\end{equation}
$$

Let's recap what we've accomplished so far with this definition:
- We've verified that it works for all of the ideas that our old definitions worked for
- We've shown that it is much simpler and faster to use than our old definition
- We've noted that it breaks free from the restrictions of the old definition, even though it still gives the same results

## Part 4: Breaking free
Now we that we've established that our new definition is free from the restrictions of the old one, what can we do with it? Let's try to use some fractional powers:

$$
\begin{equation}
\begin{aligned}
& 3^{\frac{1}{2}} \times 3^{\frac{1}{2}} = 3^{\frac{1}{2}+\frac{1}{2}} \\
& 3^{\frac{1}{2}} \times 3^{\frac{1}{2}} = 3^{1} \\
& 3^{\frac{1}{2}} \times 3^{\frac{1}{2}} = 3 \\
\end{aligned}
\end{equation}
$$

Wait a second. We just multiplied this unknown number $3^{\frac{1}{2}}$ by itself, and then got 3 back. That's pretty weird, but it's actually the same as something else you've seen before:

$$
\begin{equation}
\begin{aligned}
& \sqrt{3} \times \sqrt{3} = 3
\end{aligned}
\end{equation}
$$

You might remember that the definition of a square root is that when you multiply it by itself, you get the number under the square root. So if we were to represent it with a power, then it should just be half of one, which is what we saw earlier. NOTE: I feel like I could justify this better but I don't know how to word it




- TODO: Talk about cube roots
- TODO: Talk about other non integer powers, with examples such as compound interest
- TODO: talk about how extending definitions means examples and analogies might break down/not be general enough
- TODO: figure out equation numbers in latex
- TODO: figure fix formatting on year 1, year 2, year 3...

