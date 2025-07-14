

- Swift
- UInt
-  UInt.SIMD64Storage 

Structure

# UInt.SIMD64Storage

Storage for a vector of 64 integers.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct SIMD64Storage
```

## Topics

### Initializers

init()

Creates a vector with zero in all lanes.

### Instance Properties

var scalarCount: Int

The number of scalars, or elements, in the vector.

### Subscripts

subscript(Int) -> UInt

Accesses the element at the specified index.

### Type Aliases

typealias Scalar

## Relationships

### Conforms To

- BitwiseCopyable
- SIMDStorage
- Sendable

