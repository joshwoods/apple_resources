

- Metal Performance Shaders
-  MPSAccelerationStructure Deprecated

Class

# MPSAccelerationStructure

The base class for data structures that are built over geometry and used to accelerate ray tracing.

iOS 12.0–17.0DeprecatediPadOS 12.0–17.0DeprecatedMac Catalyst 13.0–17.0DeprecatedmacOS 10.14–14.0DeprecatedtvOS 12.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class MPSAccelerationStructure : MPSKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init?(coder: NSCoder, group: MPSAccelerationStructureGroup)

init(device: any MTLDevice)

init(group: MPSAccelerationStructureGroup)

### Instance Properties

var boundingBox: MPSAxisAlignedBoundingBox

var group: MPSAccelerationStructureGroup

var status: MPSAccelerationStructureStatus

var usage: MPSAccelerationStructureUsage

### Instance Methods

func copy(with: NSZone?, device: (any MTLDevice)?) -> Self

func copy(with: NSZone?, group: MPSAccelerationStructureGroup) -> Self

func encode(with: NSCoder)

func encodeRefit(commandBuffer: any MTLCommandBuffer)

func rebuild()

func rebuild(completionHandler: MPSAccelerationStructureCompletionHandler)

## Relationships

### Inherits From

- MPSKernel

### Conforms To

- NSCopying
- NSSecureCoding

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

class MPSInstanceAccelerationStructure

An acceleration structure built over instances of other acceleration structures.

Deprecated

class MPSTriangleAccelerationStructure

An acceleration structure built over triangles.

Deprecated

