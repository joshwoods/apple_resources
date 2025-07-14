

- Accelerate
-  DSPComplex 

Structure

# DSPComplex

A structure that represents a single-precision complex value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct DSPComplex
```

## Mentioned in 

Controlling vDSP operations with stride

Performing Fourier transforms on interleaved-complex data

## Overview

Complex data are stored as ordered pairs of floating-point numbers. Because they are stored as ordered pairs, complex vectors require address strides that are multiples of two.

## Topics

### Initializers

init()

init(real: Float, imag: Float)

### Instance Properties

var imag: Float

The imaginary part of the value.

var real: Float

The real part of the value.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable
- vDSP_DiscreteFourierTransformable

## See Also

### Data types

typealias vDSP_Length

An unsigned-integer value that represents the size of vectors and the indices of elements in vectors.

typealias vDSP_Stride

An integer value that represents the differences between indices of elements, including the lengths of strides.

typealias COMPLEX_SPLIT

struct DSPDoubleComplex

A structure that represents a double-precision complex value.

typealias DOUBLE_COMPLEX_SPLIT

struct DSPSplitComplex

A structure that represents a single-precision complex vector with the real and imaginary parts stored in separate arrays.

struct DSPDoubleSplitComplex

A structure that represents a double-precision complex vector with the real and imaginary parts stored in separate arrays.

struct VectorizableDouble

A structure that represents a double-precision real value for biquadratic filtering and discrete Fourier transforms.

struct VectorizableFloat

A structure that represents a single-precision real value for biquadratic filtering and discrete Fourier transforms.

