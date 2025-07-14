

- Metal Performance Shaders
-  MPSInstanceAccelerationStructure Deprecated

Class

# MPSInstanceAccelerationStructure

An acceleration structure built over instances of other acceleration structures.

iOS 12.0–17.0DeprecatediPadOS 12.0–17.0DeprecatedMac Catalyst 13.0–17.0DeprecatedmacOS 10.14–14.0DeprecatedtvOS 12.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class MPSInstanceAccelerationStructure : MPSAccelerationStructure
```

## Topics

### Instance Properties

var accelerationStructures: [MPSPolygonAccelerationStructure]?

var instanceBuffer: (any MTLBuffer)?

var instanceBufferOffset: Int

var instanceCount: Int

var maskBuffer: (any MTLBuffer)?

var maskBufferOffset: Int

var transformBuffer: (any MTLBuffer)?

var transformBufferOffset: Int

var transformType: MPSTransformType

## Relationships

### Inherits From

- MPSAccelerationStructure

## See Also

### Ray Tracing

Animating and Denoising a Raytraced Scene

Support dynamic scenes and denoising by extending your ray tracer with Metal Performance Shaders.

class MPSRayIntersector

A kernel that performs intersection tests between rays and geometry.

Deprecated

class MPSAccelerationStructureGroup

A group of acceleration structures.

Deprecated

class MPSTriangleAccelerationStructure

An acceleration structure built over triangles.

Deprecated

class MPSAccelerationStructure

The base class for data structures that are built over geometry and used to accelerate ray tracing.

Deprecated

