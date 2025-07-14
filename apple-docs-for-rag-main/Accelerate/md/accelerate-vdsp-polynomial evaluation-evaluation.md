

- Accelerate
- vDSP
-  Polynomial evaluation 

API Collection

# Polynomial evaluation

Evaluate polynomials using coefficients and independent variables that you supply.

## Topics

### Single-precision polynomial evaluation

static func evaluatePolynomial&lt;U>(usingCoefficients: [Float], withVariables: U) -> [Float]

Returns a single-precision evaluated polynomial using specified coefficients and variables.

static func evaluatePolynomial&lt;U, V>(usingCoefficients: [Float], withVariables: U, result: inout V)

Evaluates a single-precision polynomial using specified coefficients and variables.

vDSP_vpoly

Evaluates a single-precision polynomial using specified coefficients, variables, and strides.

### Double-precision polynomial evaluation

static func evaluatePolynomial&lt;U>(usingCoefficients: [Double], withVariables: U) -> [Double]

Returns a double-precision evaluated polynomial using specified coefficients and variables.

static func evaluatePolynomial&lt;U, V>(usingCoefficients: [Double], withVariables: U, result: inout V)

Evaluates a double-precision polynomial using specified coefficients and variables.

vDSP_vpolyD

Evaluates a double-precision polynomial using specified coefficients, variables, and strides.

## See Also

### Vector-vector arithmetic

Vector-vector real arithmetic functions

Perform element-wise operations on vectors of real values.

Complex basic arithmetic

Perform elementwise operations on vectors of complex values.

Integer arithmetic

Perform elementwise operations on vectors of integer values.

Linear averaging functions

Calculate the element-wise linear average of two vectors.

