

- Accelerate
- vDSP
-  Complex conjugation functions 

API Collection

# Complex conjugation functions

Calculate the complex conjugate of the elements in a vector.

## Topics

### Single-Vector Complex Conjugation

The functions in this group find the complex conjugate of values in a vector.

static func conjugate(DSPSplitComplex, count: Int, result: inout DSPSplitComplex)

Calculates the complex conjugate of the values in a single-precision vector.

static func conjugate(DSPDoubleSplitComplex, count: Int, result: inout DSPDoubleSplitComplex)

Calculates the complex conjugate of the values in a double-precision vector.

vDSP_zvconj

Calculates the complex conjugate of the values in a single-precision vector using the specified stride.

vDSP_zvconjD

Calculates the complex conjugate of the values in a double-precision vector using the specified stride.

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

Vector squaring functions

Compute the square, signed square, or squared magnitude of the elements in a vector.

Fractional part extraction

Truncate the elements of a vector to a fraction.

Zero crossing search

Count and find the zero crossings in a vector.

