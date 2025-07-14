

- Accelerate
- vDSP
-  Vector-to-vector minima and maxima 

API Collection

# Vector-to-vector minima and maxima

Compute the element-wise minimum or maximum values or magnitudes in a vector.

## Topics

### Vector-to-Vector Minima

static func minimum&lt;U>(U, U) -> [Double]

Returns a double-precision array containing the minimum of the corresponding values of two vectors.

static func minimum&lt;U>(U, U) -> [Float]

Returns a single-precision array containing the minimum of the corresponding values of two vectors.

static func minimum&lt;U, V>(U, U, result: inout V)

Calculates the double-precision minimum of the corresponding values of two vectors.

static func minimum&lt;U, V>(U, U, result: inout V)

Calculates the single-precision minimum of the corresponding values of two vectors.

vDSP_vmin

Calculates the single-precision minimum of the corresponding values of two vectors using specified strides.

vDSP_vminD

Calculates the double-precision minimum of the corresponding values of two vectors using specified strides.

vDSP_vminmg

Calculates the single-precision minimum magnitude of the corresponding values of two vectors using specified strides.

vDSP_vminmgD

Calculates the double-precision minimum magnitude of the corresponding values of two vectors using specified strides.

### Vector-to-Vector Maxima

static func maximum&lt;U>(U, U) -> [Double]

Returns a double-precision array containing the maximum of the corresponding values of two vectors.

static func maximum&lt;U>(U, U) -> [Float]

Returns a single-precision array containing the maximum of the corresponding values of two vectors.

static func maximum&lt;U, V>(U, U, result: inout V)

Calculates the maximum of the corresponding double-precision values of two vectors.

static func maximum&lt;U, V>(U, U, result: inout V)

Calculates the maximum of the corresponding single-precision values of two vectors.

vDSP_vmax

Calculates the single-precision maximum of the corresponding values of two vectors using specified strides.

vDSP_vmaxD

Calculates the double-precision maximum of the corresponding values of two vectors using specified strides.

vDSP_vmaxmg

Calculates the single-precision maximum magnitude of the corresponding values of two vectors using specified strides.

vDSP_vmaxmgD

Calculates the double-precision maximum magnitude of the corresponding values of two vectors using specified strides.

## See Also

### Vector-to-vector extrema functions

Extrema finding functions

Extract the values from a vector that fall outside a range.

