

- Swift
- Float16
-  Float16.SIMD8Storage 

Structure

# Float16.SIMD8Storage

Storage for a vector of eight floating-point values.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@frozen
struct SIMD8Storage
```

## Topics

### Initializers

init()

Creates a vector with zero in all lanes.

### Instance Properties

var scalarCount: Int

The number of scalars, or elements, in the vector.

### Subscripts

subscript(Int) -> Float16

Accesses the element at the specified index.

### Type Aliases

typealias Scalar

## Relationships

### Conforms To

- BitwiseCopyable
- SIMDStorage
- Sendable

