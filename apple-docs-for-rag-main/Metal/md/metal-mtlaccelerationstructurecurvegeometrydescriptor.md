

- Metal
-  MTLAccelerationStructureCurveGeometryDescriptor 

Class

# MTLAccelerationStructureCurveGeometryDescriptor

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class MTLAccelerationStructureCurveGeometryDescriptor
```

## Mentioned in 

Improving Ray-Tracing Data Access Using Per-Primitive Data

## Topics

### Instance Properties

var controlPointBuffer: (any MTLBuffer)?

var controlPointBufferOffset: Int

var controlPointCount: Int

var controlPointFormat: MTLAttributeFormat

var controlPointStride: Int

var curveBasis: MTLCurveBasis

var curveEndCaps: MTLCurveEndCaps

var curveType: MTLCurveType

var indexBuffer: (any MTLBuffer)?

var indexBufferOffset: Int

var indexType: MTLIndexType

var radiusBuffer: (any MTLBuffer)?

var radiusBufferOffset: Int

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

### Geometry Descriptors

class MTLAccelerationStructureGeometryDescriptor

A base class for descriptors that contain geometry data to convert into a ray-tracing acceleration structure.

class MTLAccelerationStructureTriangleGeometryDescriptor

A description of a list of triangle primitives to turn into an acceleration structure.

enum MTLCurveType

enum MTLCurveBasis

enum MTLCurveEndCaps

class MTLAccelerationStructureBoundingBoxGeometryDescriptor

A description of a list of bounding boxes to turn into an acceleration structure.

