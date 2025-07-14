

- Accelerate
- vDSP
-  Recursive filters 

API Collection

# Recursive filters

Perform two-pole two-zero recursive filtering on a vector.

## Topics

### Vector-to-Vector Recursive Filtering on Real Vectors

static func twoPoleTwoZeroFilter&lt;U>(U, coefficients: (Double, Double, Double, Double, Double)) -> [Double]

Returns the result of double-precision, two-pole, two-zero recursive filtering.

static func twoPoleTwoZeroFilter&lt;U>(U, coefficients: (Float, Float, Float, Float, Float)) -> [Float]

Returns the result of single-precision, two-pole, two-zero recursive filtering.

static func twoPoleTwoZeroFilter&lt;U, V>(U, coefficients: (Double, Double, Double, Double, Double), result: inout V)

Performs double-precision, two-pole, two-zero recursive filtering.

static func twoPoleTwoZeroFilter&lt;U, V>(U, coefficients: (Float, Float, Float, Float, Float), result: inout V)

Performs single-precision, two-pole, two-zero recursive filtering.

vDSP_deq22

Performs two-pole two-zero recursive filtering on a single-precision vector.

vDSP_deq22D

Performs two-pole two-zero recursive filtering on a double-precision vector.

## See Also

### Vector filtering

Biquadratic IIR filters

Apply biquadratic filters to single-channel and multichannel data.

Single-channel biquadratic filters

Filter a single-channel signal with a cascade of biquadratic sections.

Multichannel biquadratic filters

Filter a multichannel signal with a cascade of biquadratic sections.

Finite impulse response filters

Perform finite impulse response filtering with decimation and antialiasing on vectors of real or complex values.

