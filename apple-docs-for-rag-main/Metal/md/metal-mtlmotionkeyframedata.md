

- Metal
-  MTLMotionKeyframeData 

Class

# MTLMotionKeyframeData

Geometry data for a specific keyframe to use in a moving object.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
class MTLMotionKeyframeData
```

## Overview

A MTLMotionKeyframeData object describes the location of geometry data for a keyframe. The exact type of data can vary, depending on which kind of motion descriptor you create. For a MTLAccelerationStructureMotionBoundingBoxGeometryDescriptor object, the buffer data is a list of bounding boxes. For a MTLAccelerationStructureMotionTriangleGeometryDescriptor, the buffer data is a list of vertices.

## Topics

### Specifying the Keyframe Data

var buffer: (any MTLBuffer)?

The buffer that holds the geometry data.

var offset: Int

The offset, in bytes, to the keyframe data.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Motion Geometry Descriptors

class MTLAccelerationStructureMotionTriangleGeometryDescriptor

A description of a list of triangle primitives, as motion keyframe data, to turn into an acceleration structure.

class MTLAccelerationStructureMotionCurveGeometryDescriptor

class MTLAccelerationStructureMotionBoundingBoxGeometryDescriptor

A description of a list of bounding boxes, as motion keyframe data, to turn into an acceleration structure.

