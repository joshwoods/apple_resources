

- Swift
- Int
-  Int.SIMD4Storage 

Structure

# Int.SIMD4Storage

Storage for a vector of four integers.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct SIMD4Storage
```

## Topics

### Initializers

init()

Creates a vector with zero in all lanes.

### Instance Properties

var scalarCount: Int

The number of scalars, or elements, in the vector.

### Subscripts

subscript(Int) -> Int

Accesses the element at the specified index.

### Type Aliases

typealias Scalar

## Relationships

### Conforms To

- BitwiseCopyable
- SIMDStorage
- Sendable

## See Also

### SIMD-Supporting Types

typealias SIMDMaskScalar

struct SIMD2Storage

Storage for a vector of two integers.

struct SIMD8Storage

Storage for a vector of eight integers.

struct SIMD16Storage

Storage for a vector of 16 integers.

struct SIMD32Storage

Storage for a vector of 32 integers.

struct SIMD64Storage

Storage for a vector of 64 integers.

