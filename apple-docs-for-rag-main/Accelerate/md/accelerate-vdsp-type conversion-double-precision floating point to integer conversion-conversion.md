

- Accelerate
- vDSP
- Type conversion
-  Double-precision floating point to integer conversion 

API Collection

# Double-precision floating point to integer conversion

Perform element-wise double-precision floating-point to integer conversion.

## Topics

### Floating point to integer conversion

static func floatingPointToInteger&lt;T, U>(T, integerType: U.Type, rounding: vDSP.RoundingMode) -> [U]

Returns double-precision values converted to integer values.

enum RoundingMode

Floating point to integer conversion rounding modes.

### Floating point to 8-bit integer conversion

static func convertElements&lt;U, V>(of: U, to: inout V, rounding: vDSP.RoundingMode)

Converts double-precision values to 8-bit signed integers.

static func convertElements&lt;U, V>(of: U, to: inout V, rounding: vDSP.RoundingMode)

Converts double-precision values to 8-bit unsigned integers.

enum RoundingMode

Floating point to integer conversion rounding modes.

vDSP_vfix8D

Converts a vector of double-precision floating-point values to signed 8-bit integer values, and rounds towards zero.

vDSP_vfixr8D

Converts a vector of double-precision floating-point values to signed 8-bit integer values, and rounds towards the nearest integer.

vDSP_vfixu8D

Converts a vector of double-precision floating-point values to unsigned 8-bit integer values, and rounds towards zero.

vDSP_vfixru8D

Converts a vector of double-precision floating-point values to unsigned 8-bit integer values, and rounds towards the nearest integer.

### Floating point to 16-bit integer conversion

static func convertElements&lt;U, V>(of: U, to: inout V, rounding: vDSP.RoundingMode)

Converts double-precision values to 16-bit signed integers.

static func convertElements&lt;U, V>(of: U, to: inout V, rounding: vDSP.RoundingMode)

Converts double-precision values to 16-bit unsigned integers.

enum RoundingMode

Floating point to integer conversion rounding modes.

vDSP_vfix16D

Converts a vector of double-precision floating-point values to signed 16-bit integer values, and rounds towards zero.

vDSP_vfixr16D

Converts a vector of double-precision floating-point values to signed 16-bit integer values, and rounds towards the nearest integer.

vDSP_vfixu16D

Converts a vector of double-precision floating-point values to unsigned 16-bit integer values, and rounds towards zero.

vDSP_vfixru16D

Converts a vector of double-precision floating-point values to unsigned 16-bit integer values, and rounds towards the nearest integer.

### Floating point to 32-bit integer conversion

static func convertElements&lt;U, V>(of: U, to: inout V, rounding: vDSP.RoundingMode)

Converts double-precision values to 32-bit signed integers.

static func convertElements&lt;U, V>(of: U, to: inout V, rounding: vDSP.RoundingMode)

Converts double-precision values to 32-bit unsigned integers.

enum RoundingMode

Floating point to integer conversion rounding modes.

vDSP_vfix32D

Converts a vector of double-precision floating-point values to signed 32-bit integer values, and rounds towards zero.

vDSP_vfixr32D

Converts a vector of double-precision floating-point values to signed 32-bit integer values, and rounds towards the nearest integer.

vDSP_vfixu32D

Converts a vector of double-precision floating-point values to unsigned 32-bit integer values, and rounds towards zero.

vDSP_vfixru32D

Converts a vector of double-precision floating-point values to unsigned 32-bit integer values, and rounds towards the nearest integer.

## See Also

### Conversion between floating-point and integer types

Integer to single-precision floating-point conversion

Perform element-wise integer to single-precision floating-point conversion.

Integer to double-precision floating-point conversion

Perform element-wise integer to double-precision floating-point conversion.

Single-precision floating point to integer conversion

Perform element-wise single-precision floating-point to integer conversion.

