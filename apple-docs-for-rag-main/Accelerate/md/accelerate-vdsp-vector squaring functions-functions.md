

- Accelerate
- vDSP
-  Vector squaring functions 

API Collection

# Vector squaring functions

Compute the square, signed square, or squared magnitude of the elements in a vector.

## Topics

### Single-Vector Squaring

The functions in this group compute the square of each element in a vector or the square of the magnitude of each element in a complex vector.

static func square&lt;U>(U) -> [Double]

Returns a double-precision array containing the square of each element in the supplied vector.

static func square&lt;U>(U) -> [Float]

Returns a single-precision array containing the square of each element in the supplied vector.

static func square&lt;U, V>(U, result: inout V)

Calculates the square of each element in the supplied double-precision vector.

static func square&lt;U, V>(U, result: inout V)

Calculates the square of each element in the supplied single-precision vector.

static func signedSquare&lt;U>(U) -> [Double]

Returns a double-precision array containing the signed square of each element in the supplied vector.

static func signedSquare&lt;U>(U) -> [Float]

Returns a single-precision array containing the signed square of each element in the supplied vector.

static func signedSquare&lt;U, V>(U, result: inout V)

Calculates the signed square of each element in the supplied double-precision vector.

static func signedSquare&lt;U, V>(U, result: inout V)

Calculates the signed square of each element in the supplied single-precision vector.

static func squareMagnitudes&lt;V>(DSPSplitComplex, result: inout V)

Calculates the square magnitude of each element in the supplied single-precision complex vector.

static func squareMagnitudes&lt;V>(DSPDoubleSplitComplex, result: inout V)

Calculates the square magnitude of each element in the supplied double-precision complex vector.

vDSP_vsq

Computes the squared value of each element in the supplied single-precision vector.

vDSP_vsqD

Computes the squared value of each element in the supplied double-precision vector.

vDSP_vssq

Computes the signed squared value of each element in the supplied single-precision vector.

vDSP_vssqD

Computes the signed squared value of each element in the supplied double-precision vector.

vDSP_zvmags

Computes the squared magnitude value of each element in the supplied complex single-precision vector.

vDSP_zvmagsD

Computes the squared magnitude value of each element in the supplied complex double-precision vector.

vDSP_zvmgsa

Complex vector magnitudes square and add; single precision.

vDSP_zvmgsaD

Complex vector magnitudes square and add; double precision.

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

Fractional part extraction

Truncate the elements of a vector to a fraction.

Zero crossing search

Count and find the zero crossings in a vector.

