

- Metal
-  MTLAccelerationStructureMotionCurveGeometryDescriptor 

Class

# MTLAccelerationStructureMotionCurveGeometryDescriptor

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class MTLAccelerationStructureMotionCurveGeometryDescriptor
```

## Mentioned in 

Improving Ray-Tracing Data Access Using Per-Primitive Data

## Topics

### Instance Properties

var controlPointBuffers: [MTLMotionKeyframeData]

var controlPointCount: Int

var controlPointFormat: MTLAttributeFormat

var controlPointStride: Int

var curveBasis: MTLCurveBasis

var curveEndCaps: MTLCurveEndCaps

var curveType: MTLCurveType

var indexBuffer: (any MTLBuffer)?

var indexBufferOffset: Int

var indexType: MTLIndexType

var radiusBuffers: [MTLMotionKeyframeData]

var radiusFormat: MTLAttributeFormat

var radiusStride: Int

var segmentControlPointCount: Int

var segmentCount: Int

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

class MTLAccelerationStructureMotionTriangleGeometryDescriptor

A description of a list of triangle primitives, as motion keyframe data, to turn into an acceleration structure.

class MTLAccelerationStructureMotionBoundingBoxGeometryDescriptor

A description of a list of bounding boxes, as motion keyframe data, to turn into an acceleration structure.

class MTLMotionKeyframeData

Geometry data for a specific keyframe to use in a moving object.

