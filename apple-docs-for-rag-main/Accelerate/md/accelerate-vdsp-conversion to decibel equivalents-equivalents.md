

- Accelerate
- vDSP
-  Conversion to decibel equivalents 

API Collection

# Conversion to decibel equivalents

Convert vectors that contain power or amplitude data to decibels.

## Topics

### Converting single-precision power or amplitude values to decibel values

static func amplitudeToDecibels&lt;U>(U, zeroReference: Float) -> [Float]

Returns single-precision amplitude values converted to decibels.

static func powerToDecibels&lt;U>(U, zeroReference: Float) -> [Float]

Returns single-precision power values converted to decibel values.

static func convert&lt;U, V>(amplitude: U, toDecibels: inout V, zeroReference: Float)

Converts single-precision amplitude values to decibel values.

static func convert&lt;U, V>(power: U, toDecibels: inout V, zeroReference: Float)

Converts single-precision power values to decibel values.

vDSP_vdbcon

Converts single-precision power or amplitude values to decibel values.

### Converting double-precision power or amplitude values to decibel values

static func amplitudeToDecibels&lt;U>(U, zeroReference: Double) -> [Double]

Returns double-precision amplitude values converted to decibel values.

static func powerToDecibels&lt;U>(U, zeroReference: Double) -> [Double]

Returns double-precision power values converted to decibel values.

static func convert&lt;U, V>(amplitude: U, toDecibels: inout V, zeroReference: Double)

Converts double-precision amplitude values to decibel values.

static func convert&lt;U, V>(power: U, toDecibels: inout V, zeroReference: Double)

Converts double-precision power values to decibel values.

vDSP_vdbconD

Converts single-precision power or amplitude values to decibel values.

## See Also

### Vector conversion functions

Type conversion

Perform element-wise floating-point to integer and integer to floating-point conversion.

Complex vector conversion

Perform element-wise split-complex to interleaved and interleaved to split-complex conversion.

Polar-rectangular conversion

Convert each element of a vector between radius-angle and Cartesian pairs.

