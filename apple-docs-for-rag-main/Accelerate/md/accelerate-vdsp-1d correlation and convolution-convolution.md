

- Accelerate
- vDSP
-  1D correlation and convolution 

API Collection

# 1D correlation and convolution

Use correlation to compare and convolution to combine vectors of real or complex data.

## Overview

The vDSP library provides functions that calculate the convolution and correlation of a signal and a filter. Both operations compute the sliding dot product of the filter and the section of the input signal that the filter is over. What the operation produced depends on whether the stride is positive or negative:

- With a positive stride through the filter, the correlation operation computes the similarity between the signal and the filter.

- With a negative stride through the filter, the convolution operation computes the effect of the filter on the signal. For example, to apply a low-pass filter to a signal.

## Topics

### Real Vectors

static func convolve&lt;T, U>(T, withKernel: U) -> [Double]

Returns the 1D convolution of a double-precision vector.

static func convolve&lt;T, U>(T, withKernel: U) -> [Float]

Returns the 1D convolution of a single-precision vector.

static func convolve&lt;T, U, V>(T, withKernel: U, result: inout V)

Calculates the 1D convolution of a double-precision vector.

static func convolve&lt;T, U, V>(T, withKernel: U, result: inout V)

Calculates the 1D convolution of a single-precision vector.

static func correlate&lt;T, U>(T, withKernel: U) -> [Double]

Returns the correlation of a double-precision signal vector and a filter vector.

static func correlate&lt;T, U>(T, withKernel: U) -> [Float]

Returns the correlation of a single-precision signal vector and a filter vector.

static func correlate&lt;T, U, V>(T, withKernel: U, result: inout V)

Calculates the correlation of a double-precision signal vector and a filter vector.

static func correlate&lt;T, U, V>(T, withKernel: U, result: inout V)

Calculates the correlation of a single-precision signal vector and a filter vector.

vDSP_conv

Performs either correlation or convolution on two real single-precision vectors.

vDSP_convD

Performs either correlation or convolution on two real double-precision vectors.

### Complex Vectors

vDSP_zconv

Performs either correlation or convolution on two complex single-precision vectors.

vDSP_zconvD

Performs either correlation or convolution on two complex double-precision vectors.

## See Also

### Vector and matrix correlation and convolution

2D convolution

Perform convolution operations on matrices of real data.

