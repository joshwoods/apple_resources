

- Kernel
- Kernel Data Types
-  DSPDoubleComplex 

Type Alias

# DSPDoubleComplex

Used to hold a double-precision complex value.

macOS 10.13+

``` source
typedef struct DSPDoubleComplex DSPDoubleComplex;
```

## Discussion

Double complex data are stored as ordered pairs of double-precision floating-point numbers. Because they are stored as ordered pairs, complex vectors require address strides that are multiples of two.

## Topics

### Fields

real

The real part of the value.

imag

The imaginary part of the value.

### Instance Properties

imag

