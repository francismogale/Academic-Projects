# Roots-of-a-Quadratics-functon

import math
def roots(a, b, c):
"""Using python to calculate the roots(x) of a quadratic function: ax^2 + bx + c = 0.
 roots(a, b, c) # input values of a, b and c to get the roots of a function """
    k = math.sqrt(math.pow(b, 2) - 4*a*c)
    x1 = -b + k/2*a if k >= 0 else complex(-b/2*a, \
        -(math.sqrt(abs(math.pow(b, 2) - 4*a*c)/2*a)))
    x2 = -b - k/2*a if k >= 0 else complex(-b/2*a, \
        -(math.sqrt(abs(math.pow(b, 2) - 4*a*c)/2*a)))
    return (x1, x2)
