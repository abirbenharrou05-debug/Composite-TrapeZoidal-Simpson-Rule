# Numerical Integration: Composite Trapezoidal and Simpson Rules

### Author: Abir Ben Harrou
### Course: Mathematics for AI
### Date: 11/10/2026

## Description

This project implements two numerical integration algorithms from the course:

1. **Composite Trapezoidal Rule**: approximates f by straight lines on each subinterval.
2. **Composite Simpson Rule**: approximates f by parabolas over pairs of subintervals (requires an even number of subintervals *n*).

Both are compared against a reference value computed with `scipy.integrate.quad`.

## Requirements

- Python 3.x
- NumPy
- SciPy

## Conclusion

In this assignment, we implemented the Composite Trapezoidal Rule and the Composite Simpson Rule and compared them against a reference value computed with scipy.integrate.quad. The trapezoidal rule approximates the function by straight lines on each subinterval, while Simpson’s rule fits parabolas over pairs of subintervals, which requires an even number of subintervals n. As a result, the trapezoidal rule has an error of order O(h²), whereas Simpson’s rule has an error of order O(h⁴), so its error decreases much faster as n increases.

For the test function f(x) = x³ on [1, 2] with n = 4, the trapezoidal rule gave an absolute error of 0.046875, while Simpson’s rule was exact up to rounding error.
