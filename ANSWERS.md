Our goal was to find functions that would break the Bisection, Newton, or Brent method.

For the Brent method, the functions that break it are those where you give an interval that has the same sign at both end points. For example, $f(x)=x^2-4$ with the interval [-4,4] would not work.

The Newton method can be broken with a functions with a discontinuous first derivative ($f(x)=\mid x \mid^\frac{1}{3}$). However, we determined that this is only an issue when the exponent is less than 1/2. It can also be broken by functions with a high number of oscillations such as $f(x)=x^6\mathrm{sin}(x)$. This happens because the secants end up intersecting other areas of the curve instead of focusing in on one root.

The Bisection method is also broken when the values of the function at the interval endpoints is the same. I also found that in some cases, it does not check the sign, so if you gave it $f(x)=x^2-4$ with the interval [-4,4], it would just give you the lower of the two roots. If the interval contains many roots, it will only return one of the roots, but you can't be sure which one it has returned. In general, if you have an idea of the interval in which the root occurs, bisection will almost always work.

