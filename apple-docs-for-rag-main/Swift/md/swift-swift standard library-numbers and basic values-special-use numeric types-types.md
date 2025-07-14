

- Swift
- Swift Standard Library
- Numbers and Basic Values
-  Special-Use Numeric Types 

API Collection

# Special-Use Numeric Types

Work with fixed-width numeric types of different sizes.

## Topics

### Unsigned Integers

struct UInt

An unsigned integer value type.

struct UInt8

An 8-bit unsigned integer value type.

struct UInt16

A 16-bit unsigned integer value type.

struct UInt32

A 32-bit unsigned integer value type.

struct UInt64

A 64-bit unsigned integer value type.

struct UInt128

A 128-bit unsigned integer value type.

### Signed Integers

struct Int8

An 8-bit signed integer value type.

struct Int16

A 16-bit signed integer value type.

struct Int32

A 32-bit signed integer value type.

struct Int64

A 64-bit signed integer value type.

struct Int128

A 128-bit signed integer value type.

### Casting Between Integer Types

func numericCast&lt;T, U>(T) -> U

Returns the given integer as the equivalent value in a different integer type.

### Floating-Point Values

struct Float16

A half-precision (16b), floating-point value type.

struct Float80

An extended-precision, floating-point value type.

### Floating-Point Type Aliases

typealias Float32

A 32-bit floating point type.

typealias Float64

A 64-bit floating point type.

## See Also

### Advanced Numerics

Numeric Protocols

Write generic code that works with any numeric type.

SIMD Vector Types

Work with fixed-width vectors of fixed-width numeric types of different sizes.

Global Numeric Functions

Use these functions with numeric values and other comparable types.

