

- Kernel
- Kernel Data Types
-  DSPComplex 

Type Alias

# DSPComplex

Used to hold a complex value.

macOS 10.13+

``` source
typedef struct DSPComplex DSPComplex;
```

## Discussion

Complex data are stored as ordered pairs of floating-point numbers. Because they are stored as ordered pairs, complex vectors require address strides that are multiples of two.

## Topics

### Fields

real

The real part of the value.

imag

The imaginary part of the value.

### Instance Properties

imag

