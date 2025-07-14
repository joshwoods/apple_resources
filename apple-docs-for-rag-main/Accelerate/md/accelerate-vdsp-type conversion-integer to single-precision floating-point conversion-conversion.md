

- Accelerate
- vDSP
- Type conversion
-  Integer to single-precision floating-point conversion 

API Collection

# Integer to single-precision floating-point conversion

Perform element-wise integer to single-precision floating-point conversion.

## Topics

### 8-bit integer to floating point conversion

The functions in this group convert integer values of a given size to floating-point vectors.

static func integerToFloatingPoint&lt;T, U>(T, floatingPointType: U.Type) -> [U]

Returns a vector of floating-point values converted from signed 8-bit integer values.

static func integerToFloatingPoint&lt;T, U>(T, floatingPointType: U.Type) -> [U]

Returns a vector of floating-point values converted from unsigned 8-bit integer values.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts 8-bit signed integers to single-precision values.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts 8-bit unsigned integers to single-precision values.

vDSP_vflt8

Converts a vector of signed 8-bit integers to single-precision floating-point values.

vDSP_vfltu8

Converts an array of unsigned 8-bit integers to single-precision floating-point values.

### 16-bit integer to floating point conversion

static func integerToFloatingPoint&lt;T, U>(T, floatingPointType: U.Type) -> [U]

Returns a vector of floating-point values converted from signed 16-bit integer values.

static func integerToFloatingPoint&lt;T, U>(T, floatingPointType: U.Type) -> [U]

Returns a vector of floating-point values converted from unsigned 16-bit integer values.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts 16-bit signed integers to single-precision values.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts 16-bit unsigned integers to single-precision values.

vDSP_vflt16

Converts a vector of signed 16-bit integers to single-precision floating-point values.

vDSP_vfltu16

Converts an array of unsigned 16-bit integers to single-precision floating-point values.

### 24-bit integer to floating point conversion

vDSP_vflt24

Converts a vector of signed 24-bit integers to single-precision floating-point values.

vDSP_vfltu24

Converts a vector of unsigned 24-bit integers to single-precision floating-point values.

vDSP_vfltsm24

Converts and scales a vector of signed 24-bit integers to single-precision floating-point values.

vDSP_vfltsmu24

Converts and scales a vector of unsigned 24-bit integers to single-precision floating-point values.

struct vDSP_int24

A data structure that holds a 24-bit signed integer value.

struct vDSP_uint24

A data structure that holds a 24-bit unsigned integer value.

### 32-bit integer to floating point conversion

static func integerToFloatingPoint&lt;T, U>(T, floatingPointType: U.Type) -> [U]

Returns a vector of floating-point values converted from signed 32-bit integer values.

static func integerToFloatingPoint&lt;T, U>(T, floatingPointType: U.Type) -> [U]

Returns a vector of floating-point values converted from unsigned 32-bit integer values.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts 32-bit signed integers to single-precision values.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts 32-bit unsigned integers to single-precision values.

vDSP_vflt32

Converts a vector of signed 32-bit integers to single-precision floating-point values.

vDSP_vfltu32

Converts an array of unsigned 16-bit integers to single-precision floating-point values.

## See Also

### Conversion between floating-point and integer types

Integer to double-precision floating-point conversion

Perform element-wise integer to double-precision floating-point conversion.

Single-precision floating point to integer conversion

Perform element-wise single-precision floating-point to integer conversion.

Double-precision floating point to integer conversion

Perform element-wise double-precision floating-point to integer conversion.

