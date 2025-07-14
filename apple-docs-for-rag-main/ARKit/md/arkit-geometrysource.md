

- ARKit
-  GeometrySource 

Structure

# GeometrySource

A container for geometrical vector data.

visionOS 1.0+

``` source
struct GeometrySource
```

## Overview

Mesh-anchor geometry (MeshDescriptor) uses geometry sources to hold 3D data like vertices and normals in an efficent, array-like format. A Metal buffer wraps the data and other properties specify how to interpret that data.

If componentsPerVector is greater than one, the element type of the geometry-source array is itself a sequence (pairs, triplets, and so on).

## Topics

### Inspecting geometry data

var buffer: any MTLBuffer

A Metal buffer that contains per-vector data for a geometry source.

var count: Int

The number of vectors in a geometry source.

var format: MTLVertexFormat

The vertex format for data in a geometry source’s buffer.

var componentsPerVector: Int

The number of scalar components in each vector in a geometry source.

var offset: Int

The offset, in bytes, from the beginning of a geometry source’s buffer.

var stride: Int

The number of bytes between one vector and another in a geometry source’s buffer.

var description: String

A textual representation of this geometry source.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Sendable

## See Also

### Geometry

struct GeometryElement

A container for vertex indices of lines or triangles.

