

- Metal
-  MTLAccelerationStructureMotionTriangleGeometryDescriptor 

Class

# MTLAccelerationStructureMotionTriangleGeometryDescriptor

A description of a list of triangle primitives, as motion keyframe data, to turn into an acceleration structure.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
class MTLAccelerationStructureMotionTriangleGeometryDescriptor
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

var vertexBuffers: [MTLMotionKeyframeData]

An array of motion keyframes, each containing triangle data.

var vertexStride: Int

The stride, in bytes, between vertices in each vertex buffer.

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

### Motion Geometry Descriptors

class MTLAccelerationStructureMotionCurveGeometryDescriptor

class MTLAccelerationStructureMotionBoundingBoxGeometryDescriptor

A description of a list of bounding boxes, as motion keyframe data, to turn into an acceleration structure.

class MTLMotionKeyframeData

Geometry data for a specific keyframe to use in a moving object.

