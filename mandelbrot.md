# Mandelbrot set
In this section we define the Mandelbrot set and give the code for visualisation in Python and JavaScript.

## A bit of history...
Thes Mandelbrot set was first investigated in the 20th century by the French mathematicians Pierre Fatou and Gaston Julia (see the [Julia Set](julia_set.md)). It was popularized in 1980 thanks the visualization of the set created by [Benoit Mandelbrot](https://en.wikipedia.org/wiki/Benoit_Mandelbrot), who worked at IBM at the time.

## Mathematical definition
The Mandelbrot set is defined as the set of complex numbers $$c$$ where the function $$f_c(z) = z^2 +c$$ remains bounded when iterated in zero.

Less formally, it is all the complex numbers for which the sequence

$$ f_c(0),\quad f_c(f_c(0)),\quad f_c(f_c(f_c(0))), \ldots $$

doesn't goes to infinity and is bounded by a certain value.

Knowing that $$f_c(z) = z^2 + c$$, we can write the sequence as

$$ c,\quad c^2 + c,\quad (c^2+c)^2 + c, \ldots $$


## Graphical representation
To represent this set, we need to compute the sequence for each number and then plot the boundaries of the set.
In order to have a graphical representation, we need a way of displaying a single complex number $$c$$ in 2 dimensions.
Fortunately, we know that any complex number $$c$$ can be written as number with a real part ($$a$$) and an imaginary part ($$b$$)

$$ c = a + bi \text{.}$$

From here, two dimensional representation is straightforward. We plot the real part of the number on the x-axis and the imaginary part on the y-axis. This gives us a grif to represent any complex number. As a example the image below display two complex numbers $$z_1$$ and $$z_2$$ using this representation technique.

[Complex representation in two dimensions](Complex.svg)







