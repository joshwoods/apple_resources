

- Swift
- Double
-  Double.SIMD32Storage 

Structure

# Double.SIMD32Storage

Storage for a vector of 32 floating-point values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct SIMD32Storage
```

## Topics

### Initializers

init()

Creates a vector with zero in all lanes.

### Instance Properties

var scalarCount: Int

The number of scalars, or elements, in the vector.

### Subscripts

subscript(Int) -> Double

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

Storage for a vector of two floating-point values.

struct SIMD4Storage

Storage for a vector of four floating-point values.

struct SIMD8Storage

Storage for a vector of eight floating-point values.

struct SIMD16Storage

Storage for a vector of 16 floating-point values.

struct SIMD64Storage

Storage for a vector of 64 floating-point values.

