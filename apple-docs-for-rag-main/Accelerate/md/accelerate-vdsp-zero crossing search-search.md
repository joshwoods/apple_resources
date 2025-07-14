

- Accelerate
- vDSP
-  Zero crossing search 

API Collection

# Zero crossing search

Count and find the zero crossings in a vector.

## Topics

### Single-Vector Zero Crossing Search

The functions in this group find a specified number of zero crossings, returning the last crossing found and the number of crossings found.

static func countZeroCrossings&lt;U>(U) -> UInt

Returns the number of zero crossings in a double-precision vector.

static func countZeroCrossings&lt;U>(U) -> UInt

Returns the number of zero crossings in a single-precision vector.

vDSP_nzcros

Counts and finds the zero crossings in a single-precision vector.

vDSP_nzcrosD

Counts and finds the zero crossings in a double-precision vector.

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

Fractional part extraction

Truncate the elements of a vector to a fraction.

