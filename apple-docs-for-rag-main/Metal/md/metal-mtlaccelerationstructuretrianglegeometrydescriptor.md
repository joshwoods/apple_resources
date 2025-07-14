

- Metal
-  MTLAccelerationStructureTriangleGeometryDescriptor 

Class

# MTLAccelerationStructureTriangleGeometryDescriptor

A description of a list of triangle primitives to turn into an acceleration structure.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
class MTLAccelerationStructureTriangleGeometryDescriptor
```

## Mentioned in 

Improving Ray-Tracing Data Access Using Per-Primitive Data

## Topics

### Specifying the Number of Triangles

var triangleCount: Int

The number of triangles in the buffers.

### Specifying Index Data

var indexBuffer: (any MTLBuffer)?

A buffer that contains indices for the vertices that compose the triangle list.

var indexType: MTLIndexType

The data type of indices in the index buffer.

var indexBufferOffset: Int

The offset, in bytes, to the first index in the buffer.

### Specifying Vertex Data

var vertexBuffer: (any MTLBuffer)?

A buffer that contains vertex data.

var vertexBufferOffset: Int

The offset, in bytes, for the first vertex in the vertex buffer.

var vertexStride: Int

The stride, in bytes, between vertices in the vertex buffer.

### Instance Properties

var transformationMatrixBuffer: (any MTLBuffer)?

var transformationMatrixBufferOffset: Int

var transformationMatrixLayout: MTLMatrixLayout

var vertexFormat: MTLAttributeFormat

## Relationships

### Inherits From

- MTLAccelerationStructureGeometryDescriptor

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Geometry Descriptors

class MTLAccelerationStructureGeometryDescriptor

A base class for descriptors that contain geometry data to convert into a ray-tracing acceleration structure.

class MTLAccelerationStructureCurveGeometryDescriptor

enum MTLCurveType

enum MTLCurveBasis

enum MTLCurveEndCaps

class MTLAccelerationStructureBoundingBoxGeometryDescriptor

A description of a list of bounding boxes to turn into an acceleration structure.

