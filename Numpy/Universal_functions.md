## Universal Function: Fast Element-wise Array Functions

NumPy provides familiar mathematical functions such as sin, cos, and exp. In NumPy, these are called “universal functions”(`ufunc`). Within NumPy, these functions operate elementwise on an array, producing an array as output.

```
In [120]: arr = np.arange(10)

In [121]: np.sqrt(arr)
Out[121]: 
array([ 0.    ,  1.    ,  1.4142,  1.7321,  2.    ,  2.2361,  2.4495,
        2.6458,  2.8284,  3.    ])

In [122]: np.exp(arr)
Out[122]: 
array([    1.    ,     2.7183,     7.3891,    20.0855,    54.5982,
         148.4132,   403.4288,  1096.6332,  2980.958 ,  8103.0839])
```



- Unary universal functions

  | Function                                            | Description                                                  |
  | --------------------------------------------------- | ------------------------------------------------------------ |
  | `abs, fabs`                                         | Compute the absolute value element-wise for integer, floating point, or complex values. Use `fabs` as a faster alternative for non-complex-valued data |
  | `sqrt`                                              | Compute the square root of each element. Equivalent to `arr ** 0.5` |
  | `square`                                            | Compute the square of each element. Equivalent to `arr ** 2` |
  | `exp`                                               | Compute the exponent ex of each element                      |
  | `log, log10, log2, log1p`                           | Natural logarithm (base *e*), log base 10, log base 2, and log(1 + x), respectively |
  | `sign`                                              | Compute the sign of each element: 1 (positive), 0 (zero), or -1 (negative) |
  | `ceil`                                              | Compute the ceiling of each element, i.e. the smallest integer greater than or equal to each element |
  | `floor`                                             | Compute the floor of each element, i.e. the largest integer less than or equal to each element |
  | `rint`                                              | Round elements to the nearest integer, preserving the`dtype` |
  | `modf`                                              | Return fractional and integral parts of array as separate array |
  | `isnan`                                             | Return boolean array indicating whether each value is`NaN` (Not a Number) |
  | `isfinite, isinf`                                   | Return boolean array indicating whether each element is finite (non-`inf`, non-`NaN`) or infinite, respectively |
  | `cos, cosh, sin, sinh, tan, tanh`                   | Regular and hyperbolic trigonometric functions               |
  | `arccos, arccosh, arcsin, arcsinh, arctan, arctanh` | Inverse trigonometric functions                              |
  | `logical_not`                                       | Compute truth value of `not x` element-wise. Equivalent to `-arr`. |

- Binary universal functions

  | Function                                                     | Description                                                  |
  | ------------------------------------------------------------ | ------------------------------------------------------------ |
  | `add`                                                        | Add corresponding elements in arrays                         |
  | `subtract`                                                   | Subtract elements in second array from first array           |
  | `multiply`                                                   | Multiply array elements                                      |
  | `divide, floor_divide`                                       | Divide or floor divide (truncating the  remainder)           |
  | `power`                                                      | Raise elements in first array to powers indicated in second array |
  | `maximum, fmax`                                              | Element-wise maximum. `fmax` ignores `NaN`                   |
  | `minimum, fmin`                                              | Element-wise minimum. `fmin` ignores `NaN`                   |
  | `mod`                                                        | Element-wise modulus (remainder of division)                 |
  | `copysign`                                                   | Copy sign of values in second argument to values in first argument |
  | `greater, greater_equal, less, less_equal, equal, not_equal` | Perform element-wise comparison, yielding boolean array. Equivalent to infix operators `>, >=, <, <=, ==, !=` |
  | `logical_and, logical_or, logical_xor`                       | Compute element-wise truth value of logical operation. Equivalent to infix operators `& |, ^` |

  ​

