

- Accelerate
- vDSP
- Type conversion
-  Integer to double-precision floating-point conversion 

API Collection

# Integer to double-precision floating-point conversion

Perform element-wise integer to double-precision floating-point conversion.

## Topics

### 8-bit integer to floating point conversion

static func integerToFloatingPoint&lt;T, U>(T, floatingPointType: U.Type) -> [U]

Returns a vector of floating-point values converted from signed 8-bit integer values.

static func integerToFloatingPoint&lt;T, U>(T, floatingPointType: U.Type) -> [U]

Returns a vector of floating-point values converted from unsigned 8-bit integer values.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts 8-bit signed integers to double-precision values.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts 8-bit unsigned integers to double-precision values.

vDSP_vflt8D

Converts a vector of signed 8-bit integers to double-precision floating-point values.

vDSP_vfltu8D

Converts an array of unsigned 8-bit integers to double-precision floating-point values.

### 16-bit integer to floating point conversion

static func integerToFloatingPoint&lt;T, U>(T, floatingPointType: U.Type) -> [U]

Returns a vector of floating-point values converted from signed 16-bit integer values.

static func integerToFloatingPoint&lt;T, U>(T, floatingPointType: U.Type) -> [U]

Returns a vector of floating-point values converted from unsigned 16-bit integer values.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts 16-bit signed integers to double-precision values.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts 16-bit unsigned integers to double-precision values.

vDSP_vflt16D

Converts a vector of signed 16-bit integers to double-precision floating-point values.

vDSP_vfltu16D

Converts an array of unsigned 16-bit integers to double-precision floating-point values.

### 32-bit integer to floating point conversion

static func integerToFloatingPoint&lt;T, U>(T, floatingPointType: U.Type) -> [U]

Returns a vector of floating-point values converted from signed 32-bit integer values.

static func integerToFloatingPoint&lt;T, U>(T, floatingPointType: U.Type) -> [U]

Returns a vector of floating-point values converted from unsigned 32-bit integer values.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts 32-bit signed integers to double-precision values.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts 32-bit unsigned integers to double-precision values.

vDSP_vflt32D

Converts a vector of signed 32-bit integers to double-precision floating-point values.

vDSP_vfltu32D

Converts an array of unsigned 32-bit integers to double-precision floating-point values.

## See Also

### Conversion between floating-point and integer types

Integer to single-precision floating-point conversion

Perform element-wise integer to single-precision floating-point conversion.

Single-precision floating point to integer conversion

Perform element-wise single-precision floating-point to integer conversion.

Double-precision floating point to integer conversion

Perform element-wise double-precision floating-point to integer conversion.

