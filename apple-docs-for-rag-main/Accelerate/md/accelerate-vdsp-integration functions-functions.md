

- Accelerate
- vDSP
-  Integration functions 

API Collection

# Integration functions

Compute the running sum, Simpson, or trapezoidal integration of a vector.

## Topics

### Integration

static func integrate&lt;U>(U, using: vDSP.IntegrationRule, stepSize: Double) -> [Double]

Returns the integration of a double-precision vector using the specified rule.

static func integrate&lt;U>(U, using: vDSP.IntegrationRule, stepSize: Float) -> [Float]

Returns the integration of a single-precision vector using the specified rule.

static func integrate&lt;U, V>(U, using: vDSP.IntegrationRule, stepSize: Double, result: inout V)

Performs the integration of a double-precision using the specified rule.

static func integrate&lt;U, V>(U, using: vDSP.IntegrationRule, stepSize: Float, result: inout V)

Performs the integration of a single-precision using the specified rule.

enum IntegrationRule

Integration rules.

### Running Sum Integration

The functions in this group perform integration on the values in a vector.

vDSP_vrsum

Performs running sum integration over a single-precision vector.

vDSP_vrsumD

Performs running sum integration over a double-precision vector.

### Simpson Integration

vDSP_vsimps

Performs Simpson integration over a single-precision vector.

vDSP_vsimpsD

Performs Simpson integration over a double-precision vector.

### Trapezoidal Integration

vDSP_vtrapz

Performs trapezoidal integration over a single-precision vector.

vDSP_vtrapzD

Performs trapezoidal integration over a double-precision vector.

## See Also

### Single-vector arithmetic functions

Absolute and negation functions

Compute the absolute or negated value of each element in a vector.

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

Zero crossing search

Count and find the zero crossings in a vector.

