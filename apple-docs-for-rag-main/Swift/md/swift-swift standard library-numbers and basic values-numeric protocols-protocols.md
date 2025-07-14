

- Swift
- Swift Standard Library
- Numbers and Basic Values
-  Numeric Protocols 

API Collection

# Numeric Protocols

Write generic code that works with any numeric type.

## Topics

### Basic Arithmetic

protocol AdditiveArithmetic

A type with values that support addition and subtraction.

protocol Numeric

A type with values that support multiplication.

protocol SignedNumeric

A numeric type with a negation operation.

protocol Strideable

A type representing continuous, one-dimensional values that can be offset and measured.

### Integer

protocol BinaryInteger

An integer type with a binary representation.

protocol FixedWidthInteger

An integer type that uses a fixed size for every instance.

protocol SignedInteger

An integer type that can represent both positive and negative values.

protocol UnsignedInteger

An integer type that can represent only nonnegative values.

### Floating Point

protocol FloatingPoint

A floating-point numeric type.

protocol BinaryFloatingPoint

A radix-2 (binary) floating-point type.

### Floating-Point Characteristics

enum FloatingPointClassification

The IEEE 754 floating-point classes.

enum FloatingPointRoundingRule

A rule for rounding a floating-point number.

enum FloatingPointSign

The sign of a floating-point value.

## See Also

### Advanced Numerics

Special-Use Numeric Types

Work with fixed-width numeric types of different sizes.

SIMD Vector Types

Work with fixed-width vectors of fixed-width numeric types of different sizes.

Global Numeric Functions

Use these functions with numeric values and other comparable types.

