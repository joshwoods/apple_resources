

- Swift
-  SIMDScalar 

Protocol

# SIMDScalar

A type that can be used as an element in a SIMD vector.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol SIMDScalar : BitwiseCopyable
```

## Topics

### Associated Types

associatedtype SIMD16Storage : SIMDStorage

**Required**

associatedtype SIMD2Storage : SIMDStorage

**Required**

associatedtype SIMD32Storage : SIMDStorage

**Required**

associatedtype SIMD4Storage : SIMDStorage

**Required**

associatedtype SIMD64Storage : SIMDStorage

**Required**

associatedtype SIMD8Storage : SIMDStorage

**Required**

associatedtype SIMDMaskScalar : FixedWidthInteger, SIMDScalar, SignedInteger

**Required**

## Relationships

### Inherits From

- BitwiseCopyable

### Conforming Types

- Double
- Float
- Float16
- Int
- Int16
- Int32
- Int64
- Int8
- UInt
- UInt16
- UInt32
- UInt64
- UInt8

## See Also

### Supporting Types

protocol SIMD

A SIMD vector of a fixed number of elements.

protocol SIMDStorage

A type that can function as storage for a SIMD vector type.

struct SIMDMask

