

- Accelerate
- vDSP
- Type conversion
-  Single-precision floating point to integer conversion 

API Collection

# Single-precision floating point to integer conversion

Perform element-wise single-precision floating-point to integer conversion.

## Topics

### Floating point to integer conversion

static func floatingPointToInteger&lt;T, U>(T, integerType: U.Type, rounding: vDSP.RoundingMode) -> [U]

Returns single-precision values converted to integer values.

enum RoundingMode

Floating point to integer conversion rounding modes.

### Floating point to 8-bit integer conversion

The functions in this group convert the values in a vector from floating-point values to integer values of a given size.

static func convertElements&lt;U, V>(of: U, to: inout V, rounding: vDSP.RoundingMode)

Converts single-precision values to 8-bit signed integers.

static func convertElements&lt;U, V>(of: U, to: inout V, rounding: vDSP.RoundingMode)

Converts single-precision values to 8-bit unsigned integers.

enum RoundingMode

Floating point to integer conversion rounding modes.

vDSP_vfix8

Converts a vector of single-precision floating-point values to signed 8-bit integer values, and rounds towards zero.

vDSP_vfixr8

Converts a vector of single-precision floating-point values to signed 8-bit integer values, and rounds towards the nearest integer.

vDSP_vfixu8

Converts a vector of single-precision floating-point values to unsigned 8-bit integer values, and rounds towards zero.

vDSP_vfixru8

Converts a vector of single-precision floating-point values to unsigned 8-bit integer values, and rounds towards the nearest integer.

### Floating point to 16-bit integer conversion

static func convertElements&lt;U, V>(of: U, to: inout V, rounding: vDSP.RoundingMode)

Converts single-precision values to 16-bit signed integers.

static func convertElements&lt;U, V>(of: U, to: inout V, rounding: vDSP.RoundingMode)

Converts single-precision values to 16-bit unsigned integers.

enum RoundingMode

Floating point to integer conversion rounding modes.

vDSP_vfix16

Converts a vector of single-precision floating-point values to signed 16-bit integer values, and rounds towards zero.

vDSP_vfixr16

Converts a vector of single-precision floating-point values to signed 16-bit integer values, and rounds towards the nearest integer.

vDSP_vfixu16

Converts a vector of single-precision floating-point values to unsigned 16-bit integer values, and rounds towards zero.

vDSP_vfixru16

Converts a vector of single-precision floating-point values to unsigned 16-bit integer values, and rounds towards the nearest integer.

### Floating point to 24-bit integer conversion

The functions in this group scale and convert floating-point values to and from signed 24-bit integer values.

vDSP_vsmfix24

Converts a vector of single-precision floating-point values to signed 24-bit integer values, and rounds towards zero.

vDSP_vsmfixu24

Converts a vector of single-precision floating-point values to signed 24-bit integer values, and rounds towards the nearest integer.

struct vDSP_int24

A data structure that holds a 24-bit signed integer value.

struct vDSP_uint24

A data structure that holds a 24-bit unsigned integer value.

### Floating point to 32-bit integer conversion

static func convertElements&lt;U, V>(of: U, to: inout V, rounding: vDSP.RoundingMode)

Converts single-precision values to 32-bit signed integers.

static func convertElements&lt;U, V>(of: U, to: inout V, rounding: vDSP.RoundingMode)

Converts single-precision values to 32-bit unsigned integers.

enum RoundingMode

Floating point to integer conversion rounding modes.

vDSP_vfix32

Converts a vector of single-precision floating-point values to signed 32-bit integer values, and rounds towards zero.

vDSP_vfixr32

Converts a vector of single-precision floating-point values to signed 32-bit integer values, and rounds towards the nearest integer.

vDSP_vfixu32

Converts a vector of single-precision floating-point values to unsigned 32-bit integer values, and rounds towards zero.

vDSP_vfixru32

Converts a vector of single-precision floating-point values to unsigned 32-bit integer values, and rounds towards the nearest integer.

## See Also

### Conversion between floating-point and integer types

Integer to single-precision floating-point conversion

Perform element-wise integer to single-precision floating-point conversion.

Integer to double-precision floating-point conversion

Perform element-wise integer to double-precision floating-point conversion.

Double-precision floating point to integer conversion

Perform element-wise double-precision floating-point to integer conversion.

