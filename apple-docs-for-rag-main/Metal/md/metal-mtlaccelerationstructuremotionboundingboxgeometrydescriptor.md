

- Metal
-  MTLAccelerationStructureMotionBoundingBoxGeometryDescriptor 

Class

# MTLAccelerationStructureMotionBoundingBoxGeometryDescriptor

A description of a list of bounding boxes, as motion keyframe data, to turn into an acceleration structure.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
class MTLAccelerationStructureMotionBoundingBoxGeometryDescriptor
```

## Mentioned in 

Improving Ray-Tracing Data Access Using Per-Primitive Data

## Topics

### Specifying the Number of Bounding Boxes

var boundingBoxCount: Int

The number of bounding boxes in each bounding box buffer.

### Specifying Bounding Boxes Data

var boundingBoxBuffers: [MTLMotionKeyframeData]

A array of motion keyframes, each containing bounding box data.

var boundingBoxStride: Int

The stride, in bytes, between bounding boxes in each buffer.

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

class MTLAccelerationStructureMotionCurveGeometryDescriptor

class MTLMotionKeyframeData

Geometry data for a specific keyframe to use in a moving object.

