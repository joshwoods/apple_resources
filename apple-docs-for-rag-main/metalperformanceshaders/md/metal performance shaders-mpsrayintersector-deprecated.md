

- Metal Performance Shaders
-  MPSRayIntersector Deprecated

Class

# MPSRayIntersector

A kernel that performs intersection tests between rays and geometry.

iOS 12.0–17.0DeprecatediPadOS 12.0–17.0DeprecatedMac Catalyst 13.0–17.0DeprecatedmacOS 10.14–14.0DeprecatedtvOS 12.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class MPSRayIntersector : MPSKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice)

### Instance Properties

var boundingBoxIntersectionTestType: MPSBoundingBoxIntersectionTestType

var cullMode: MTLCullMode

var frontFacingWinding: MTLWinding

var intersectionDataType: MPSIntersectionDataType

var intersectionStride: Int

var rayDataType: MPSRayDataType

var rayIndexDataType: MPSDataType

var rayMask: UInt32

var rayMaskOperator: MPSRayMaskOperator

var rayMaskOptions: MPSRayMaskOptions

var rayStride: Int

var triangleIntersectionTestType: MPSTriangleIntersectionTestType

### Instance Methods

func copy(with: NSZone?, device: (any MTLDevice)?) -> Self

func encode(with: NSCoder)

func encodeIntersection(commandBuffer: any MTLCommandBuffer, intersectionType: MPSIntersectionType, rayBuffer: any MTLBuffer, rayBufferOffset: Int, intersectionBuffer: any MTLBuffer, intersectionBufferOffset: Int, rayCount: Int, accelerationStructure: MPSAccelerationStructure)

func encodeIntersection(commandBuffer: any MTLCommandBuffer, intersectionType: MPSIntersectionType, rayBuffer: any MTLBuffer, rayBufferOffset: Int, intersectionBuffer: any MTLBuffer, intersectionBufferOffset: Int, rayCountBuffer: any MTLBuffer, rayCountBufferOffset: Int, accelerationStructure: MPSAccelerationStructure)

func encodeIntersection(commandBuffer: any MTLCommandBuffer, intersectionType: MPSIntersectionType, rayBuffer: any MTLBuffer, rayBufferOffset: Int, rayIndexBuffer: any MTLBuffer, rayIndexBufferOffset: Int, intersectionBuffer: any MTLBuffer, intersectionBufferOffset: Int, rayIndexCount: Int, accelerationStructure: MPSAccelerationStructure)

func encodeIntersection(commandBuffer: any MTLCommandBuffer, intersectionType: MPSIntersectionType, rayBuffer: any MTLBuffer, rayBufferOffset: Int, rayIndexBuffer: any MTLBuffer, rayIndexBufferOffset: Int, intersectionBuffer: any MTLBuffer, intersectionBufferOffset: Int, rayIndexCountBuffer: any MTLBuffer, rayIndexCountBufferOffset: Int, accelerationStructure: MPSAccelerationStructure)

func encodeIntersection(commandBuffer: any MTLCommandBuffer, intersectionType: MPSIntersectionType, rayTexture: any MTLTexture, intersectionTexture: any MTLTexture, accelerationStructure: MPSAccelerationStructure)

func recommendedMinimumRayBatchSize(rayCount: Int) -> Int

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

class MPSAccelerationStructureGroup

A group of acceleration structures.

Deprecated

class MPSInstanceAccelerationStructure

An acceleration structure built over instances of other acceleration structures.

Deprecated

class MPSTriangleAccelerationStructure

An acceleration structure built over triangles.

Deprecated

class MPSAccelerationStructure

The base class for data structures that are built over geometry and used to accelerate ray tracing.

Deprecated

