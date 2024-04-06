# CLASS 3
## 1. Approximation methods
### 1.1. Simpson's rule

Basic idea:
- Given a function, we want to find the area under the curve.
- We can use Simpson's rule to do this.
- Simpson's rule is a method of numerical integration.
- What it does is to approximate the area under the curve by using a quadratic polynomial.
- We can then use the quadratic polynomial to find the area under the curve.
- We can also use the quadratic polynomial to approximate the function.

### 1.2. Cubic spline interpolation

Basic idea:
- Given a set of points, we want to find a function that passes through all of them.
- We can use a cubic spline to do this.
- A cubic spline is a piecewise function, where each piece is a cubic polynomial.
- We can find the coefficients of the cubic polynomials by solving a system of linear equations.
- We can then use the cubic polynomials to interpolate the points.
- We can also use the cubic polynomials to extrapolate the points.

#### Note:
- Find the error of the approximations.

### 1.3. Breaking into rectangles/ Reimann sum

Basic idea:
- Given a function, we want to find the area under the curve.
- We can use the Reimann sum to do this.
- The Reimann sum is a method of numerical integration.
- What it does is to approximate the area under the curve by using rectangles.
- We can then use the rectangles to find the area under the curve.
- We can also use the rectangles to approximate the function.
- The error arises due to the triangles formed by the rectangles.
- The error can be reduced by increasing the number of rectangles.
- The error reduces when the triangle is smaller i.e. the function is relatively flat

## What we do?

- Basically choose larger intervals where the function is relatively flat.
- Choose smaller intervals where the function is relatively steep.
- Design an adaptive scheme to choose the intervals.
- Interval size is `h`
- $N = \frac{b-a}{h}$
- `N` is the number of intervals

## Issues

- Multidiemensional functions: What happens is that the function is not a single variable function. Makes life harder.
- Discontinuities: The function is not continuous. Makes life harder.

## 2. Solving 1-D integral

### 2.1. Monte-Carlo method

Basic idea:
- Monte Carlo integration is a method to find intervals using random numbers.
- Computes a definite integral
- By adding up the rectangles and averaging the result, we get closer n closer to the true value
- Check out this [link](https://towardsdatascience.com/the-basics-of-monte-carlo-integration-5fe16b40482d) for more information.
- We end up with:

### $I = \frac{b-a}{N} \sum_{i=1}^{N} f(x_i)$ = $\int_{a}^{b} f(x) dx$ 
- The integral simplifies to this under Monte Carlo method.

### $I = (b-a) \int_{a}^{b} \rho(x) f(x) dx$
- here $\rho(x)$ is like a random number generator which generates random numbers between `a` and `b`.
- This approximates the area very well as N increases.
