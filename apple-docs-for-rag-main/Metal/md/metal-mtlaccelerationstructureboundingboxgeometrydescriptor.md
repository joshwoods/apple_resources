

- Metal
-  MTLAccelerationStructureBoundingBoxGeometryDescriptor 

Class

# MTLAccelerationStructureBoundingBoxGeometryDescriptor

A description of a list of bounding boxes to turn into an acceleration structure.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
class MTLAccelerationStructureBoundingBoxGeometryDescriptor
```

## Mentioned in 

Improving Ray-Tracing Data Access Using Per-Primitive Data

## Topics

### Specifying the Number of Bounding Boxes

var boundingBoxCount: Int

The number of bounding boxes in the bounding box buffer.

### Specifying Bounding Boxes Data

var boundingBoxBuffer: (any MTLBuffer)?

A buffer that contains bounding box data.

var boundingBoxBufferOffset: Int

The offset, in bytes, to the first bounding box in the buffer.

var boundingBoxStride: Int

The stride, in bytes, between bounding boxes in the buffer.

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

class MTLAccelerationStructureTriangleGeometryDescriptor

A description of a list of triangle primitives to turn into an acceleration structure.

class MTLAccelerationStructureCurveGeometryDescriptor

enum MTLCurveType

enum MTLCurveBasis

enum MTLCurveEndCaps

