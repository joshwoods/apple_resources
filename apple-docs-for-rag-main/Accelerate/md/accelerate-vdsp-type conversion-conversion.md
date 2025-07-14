

- Accelerate
- vDSP
-  Type conversion 

API Collection

# Type conversion

Perform element-wise floating-point to integer and integer to floating-point conversion.

## Topics

### Conversion between floating-point types

The functions in this group convert between single-precision and double-precision floating-point vectors.

static func doubleToFloat&lt;U>(U) -> [Float]

Returns single-precision values converted from a double-precision source.

static func floatToDouble&lt;U>(U) -> [Double]

Returns double-precision values converted from a single-precision source.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts single-precision values to double-precision values.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts double-precision values to single-precision values.

vDSP_vspdp

Converts a single-precision vector to a double-precision vector.

vDSP_vdpsp

Converts a double-precision vector to a single-precision vector.

### Conversion between floating-point and integer types

Integer to single-precision floating-point conversion

Perform element-wise integer to single-precision floating-point conversion.

Integer to double-precision floating-point conversion

Perform element-wise integer to double-precision floating-point conversion.

Single-precision floating point to integer conversion

Perform element-wise single-precision floating-point to integer conversion.

Double-precision floating point to integer conversion

Perform element-wise double-precision floating-point to integer conversion.

## See Also

### Vector conversion functions

Conversion to decibel equivalents

Convert vectors that contain power or amplitude data to decibels.

Complex vector conversion

Perform element-wise split-complex to interleaved and interleaved to split-complex conversion.

Polar-rectangular conversion

Convert each element of a vector between radius-angle and Cartesian pairs.

