

- Accelerate
- vDSP
-  Fractional part extraction 

API Collection

# Fractional part extraction

Truncate the elements of a vector to a fraction.

## Topics

### Single-Vector Fractional Part Extraction

The functions in this group remove the whole-number part of each element in a vector, leaving the fractional part in the output vector.

static func trunc&lt;U>(U) -> [Double]

Returns a double-precision array containing each element in the supplied vector truncated to a fraction.

static func trunc&lt;U>(U) -> [Float]

Returns a single-precision array containing each element in the supplied vector truncated to a fraction.

static func trunc&lt;U, V>(U, result: inout V)

Calculates each element in the supplied double-precision vector truncated to a fraction.

static func trunc&lt;U, V>(U, result: inout V)

Calculates each element in the supplied single-precision vector truncated to a fraction.

vDSP_vfrac

Truncates the elements of a single-precision vector to fractions.

vDSP_vfracD

Truncates the elements of a double-precision vector to fractions.

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

Phase computation functions

Calculate the element-wise phase values, in radians, of a complex vector.

Complex conjugation functions

Calculate the complex conjugate of the elements in a vector.

Vector squaring functions

Compute the square, signed square, or squared magnitude of the elements in a vector.

Zero crossing search

Count and find the zero crossings in a vector.

