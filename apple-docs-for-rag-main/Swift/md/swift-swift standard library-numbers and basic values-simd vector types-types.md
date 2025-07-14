

- Swift
- Swift Standard Library
- Numbers and Basic Values
-  SIMD Vector Types 

API Collection

# SIMD Vector Types

Work with fixed-width vectors of fixed-width numeric types of different sizes.

## Topics

### SIMD Vectors

struct SIMD2

A vector of two scalar values.

struct SIMD3

A vector of three scalar values.

struct SIMD4

A vector of four scalar values.

struct SIMD8

A vector of eight scalar values.

struct SIMD16

A vector of 16 scalar values.

struct SIMD32

A vector of 32 scalar values.

struct SIMD64

A vector of 64 scalar values.

### Supporting Types

protocol SIMD

A SIMD vector of a fixed number of elements.

protocol SIMDScalar

A type that can be used as an element in a SIMD vector.

protocol SIMDStorage

A type that can function as storage for a SIMD vector type.

struct SIMDMask

### Supporting Functions

func all&lt;Storage>(SIMDMask&lt;Storage>) -> Bool

True if every lane of mask is true.

func any&lt;Storage>(SIMDMask&lt;Storage>) -> Bool

True if any lane of mask is true.

func pointwiseMax&lt;T>(T, T) -> T

The lanewise maximum of two vectors.

func pointwiseMax&lt;T>(T, T) -> T

The lanewise maximum of two vectors.

func pointwiseMin&lt;T>(T, T) -> T

The lanewise minimum of two vectors.

func pointwiseMin&lt;T>(T, T) -> T

The lanewise minimum of two vectors.

## See Also

### Advanced Numerics

Numeric Protocols

Write generic code that works with any numeric type.

Special-Use Numeric Types

Work with fixed-width numeric types of different sizes.

Global Numeric Functions

Use these functions with numeric values and other comparable types.

