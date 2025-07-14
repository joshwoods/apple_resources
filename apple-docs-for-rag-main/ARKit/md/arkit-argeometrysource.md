

- ARKit
-  ARGeometrySource 

Class

# ARGeometrySource

Mesh data in a buffer-based array.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
class ARGeometrySource
```

## Overview

Mesh-anchor geometry (ARMeshGeometry) uses geometry sources to hold 3D data like vertices, and normals, in an efficent, array-like format. A Metal buffer wraps the data, and other properties specify how to interpret that data.

In the case that componentsPerVector is greater than 1, the element type of the geometry-source array is itself a sequence (pairs, triplets, and so on).

## Topics

### Accessing Geometry

subscript(Int32) -> (Float, Float, Float)

Provides the source float triplet at the subscripted index.

subscript(Int32) -> CUnsignedChar

Provides the number at the subscripted index.

var buffer: any MTLBuffer

A Metal buffer that contains a list of vectors.

### Getting Geometry Information

var componentsPerVector: Int

The number of scalar components in each vector.

var count: Int

The number of vectors in the buffer.

var format: MTLVertexFormat

The type of vector data in the buffer.

var offset: Int

The offset, in bytes, from the beginning of the buffer.

var stride: Int

The length, in bytes, of the start of one vector in the buffer to the start of the next vector.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Accessing Geometry Data

var vertices: ARGeometrySource

The vertices of the mesh.

