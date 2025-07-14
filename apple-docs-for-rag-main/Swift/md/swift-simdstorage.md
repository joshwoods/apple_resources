

- Swift
-  SIMDStorage 

Protocol

# SIMDStorage

A type that can function as storage for a SIMD vector type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol SIMDStorage
```

## Overview

The `SIMDStorage` protocol defines a storage layout and provides elementwise accesses. Computational operations are defined on the `SIMD` protocol, which refines this protocol, and on the concrete types that conform to `SIMD`.

## Topics

### Associated Types

associatedtype Scalar : Decodable, Encodable, Hashable

**Required**

### Initializers

init()

Creates a vector with zero in all lanes.

**Required**

### Instance Properties

var scalarCount: Int

The number of scalars, or elements, in the vector.

**Required** Default implementation provided.

### Subscripts

subscript(Int) -> Self.Scalar

Accesses the element at the specified index.

**Required** Default implementations provided.

## Relationships

### Inherited By

- SIMD

### Conforming Types

- Double.SIMD16Storage
- Double.SIMD2Storage
- Double.SIMD32Storage
- Double.SIMD4Storage
- Double.SIMD64Storage
- Double.SIMD8Storage
- Float.SIMD16Storage
- Float.SIMD2Storage
- Float.SIMD32Storage
- Float.SIMD4Storage
- Float.SIMD64Storage
- Float.SIMD8Storage
- Float16.SIMD16Storage
- Float16.SIMD2Storage
- Float16.SIMD32Storage
- Float16.SIMD4Storage
- Float16.SIMD64Storage
- Float16.SIMD8Storage
- Int.SIMD16Storage
- Int.SIMD2Storage
- Int.SIMD32Storage
- Int.SIMD4Storage
- Int.SIMD64Storage
- Int.SIMD8Storage
- Int16.SIMD16Storage
- Int16.SIMD2Storage
- Int16.SIMD32Storage
- Int16.SIMD4Storage
- Int16.SIMD64Storage
- Int16.SIMD8Storage
- Int32.SIMD16Storage
- Int32.SIMD2Storage
- Int32.SIMD32Storage
- Int32.SIMD4Storage
- Int32.SIMD64Storage
- Int32.SIMD8Storage
- Int64.SIMD16Storage
- Int64.SIMD2Storage
- Int64.SIMD32Storage
- Int64.SIMD4Storage
- Int64.SIMD64Storage
- Int64.SIMD8Storage
- Int8.SIMD16Storage
- Int8.SIMD2Storage
- Int8.SIMD32Storage
- Int8.SIMD4Storage
- Int8.SIMD64Storage
- Int8.SIMD8Storage
- SIMD16
- SIMD2
- SIMD3
- SIMD32
- SIMD4
- SIMD64
- SIMD8
- SIMDMask
- UInt.SIMD16Storage
- UInt.SIMD2Storage
- UInt.SIMD32Storage
- UInt.SIMD4Storage
- UInt.SIMD64Storage
- UInt.SIMD8Storage
- UInt16.SIMD16Storage
- UInt16.SIMD2Storage
- UInt16.SIMD32Storage
- UInt16.SIMD4Storage
- UInt16.SIMD64Storage
- UInt16.SIMD8Storage
- UInt32.SIMD16Storage
- UInt32.SIMD2Storage
- UInt32.SIMD32Storage
- UInt32.SIMD4Storage
- UInt32.SIMD64Storage
- UInt32.SIMD8Storage
- UInt64.SIMD16Storage
- UInt64.SIMD2Storage
- UInt64.SIMD32Storage
- UInt64.SIMD4Storage
- UInt64.SIMD64Storage
- UInt64.SIMD8Storage
- UInt8.SIMD16Storage
- UInt8.SIMD2Storage
- UInt8.SIMD32Storage
- UInt8.SIMD4Storage
- UInt8.SIMD64Storage
- UInt8.SIMD8Storage

## See Also

### Supporting Types

protocol SIMD

A SIMD vector of a fixed number of elements.

protocol SIMDScalar

A type that can be used as an element in a SIMD vector.

struct SIMDMask

