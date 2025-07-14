

- Metal
-  MTLAccelerationStructureGeometryDescriptor 

Class

# MTLAccelerationStructureGeometryDescriptor

A base class for descriptors that contain geometry data to convert into a ray-tracing acceleration structure.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
class MTLAccelerationStructureGeometryDescriptor
```

## Mentioned in 

Improving Ray-Tracing Data Access Using Per-Primitive Data

## Overview

Don’t use this base class directly. Use one of the derived classes instead, as MTLAccelerationStructure describes.

## Topics

### Specifying Base Geometry Properties

var label: String?

A label for the geometry structure, suitable for debugging.

var intersectionFunctionTableOffset: Int

An index into the intersection table for determining which intersection function Metal calls when it intersects a ray with the acceleration structure.

var opaque: Bool

A Boolean value that determines whether the geometry data in the acceleration structure needs to skip triangle-intersection tests.

var allowDuplicateIntersectionFunctionInvocation: Bool

A Boolean value that indicates whether Metal calls the ray-intersection test more than once per primitive on the structure.

### Instance Properties

var primitiveDataBuffer: (any MTLBuffer)?

var primitiveDataBufferOffset: Int

var primitiveDataElementSize: Int

var primitiveDataStride: Int

## Relationships

### Inherits From

- NSObject

### Inherited By

- MTLAccelerationStructureBoundingBoxGeometryDescriptor
- MTLAccelerationStructureCurveGeometryDescriptor
- MTLAccelerationStructureMotionBoundingBoxGeometryDescriptor
- MTLAccelerationStructureMotionCurveGeometryDescriptor
- MTLAccelerationStructureMotionTriangleGeometryDescriptor
- MTLAccelerationStructureTriangleGeometryDescriptor

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Related Documentation

class MTLAccelerationStructureMotionTriangleGeometryDescriptor

A description of a list of triangle primitives, as motion keyframe data, to turn into an acceleration structure.

class MTLAccelerationStructureMotionBoundingBoxGeometryDescriptor

A description of a list of bounding boxes, as motion keyframe data, to turn into an acceleration structure.

### Geometry Descriptors

class MTLAccelerationStructureTriangleGeometryDescriptor

A description of a list of triangle primitives to turn into an acceleration structure.

class MTLAccelerationStructureCurveGeometryDescriptor

enum MTLCurveType

enum MTLCurveBasis

enum MTLCurveEndCaps

class MTLAccelerationStructureBoundingBoxGeometryDescriptor

A description of a list of bounding boxes to turn into an acceleration structure.

