

- Accelerate
- vDSP
-  Phase computation functions 

API Collection

# Phase computation functions

Calculate the element-wise phase values, in radians, of a complex vector.

## Topics

### Single-Vector Phase Computation

The functions in this group compute the phase values of each element in a complex vector.

static func phase&lt;V>(DSPSplitComplex, result: inout V)

Calculates the single-precision element-wise phase values, in radians, of the supplied complex vector.

static func phase&lt;V>(DSPDoubleSplitComplex, result: inout V)

Calculates the double-precision element-wise phase values, in radians, of the supplied complex vector.

vDSP_zvphas

Calculates the single-precision element-wise phase values, in radians, of the supplied complex vector using the specified stride.

vDSP_zvphasD

Calculates the double-precision element-wise phase values, in radians, of the supplied complex vector using the specified stride.

## See Also

### Single-vector arithmetic functions

Absolute and negation functions

Compute the absolute or negated value of each element in a vector.

Integration functions

Compute the running sum, Simpson, or trapezoidal integration of a vector.

Clipping, limit, and threshold operations

Apply clipping, limit, or threshold rules to the elements in a vector.

Normalization functions

Compute the mean and standard deviation of a vector and calculate new elements to have a zero mean and a unit standard deviation.

Complex conjugation functions

Calculate the complex conjugate of the elements in a vector.

Vector squaring functions

Compute the square, signed square, or squared magnitude of the elements in a vector.

Fractional part extraction

Truncate the elements of a vector to a fraction.

Zero crossing search

Count and find the zero crossings in a vector.

