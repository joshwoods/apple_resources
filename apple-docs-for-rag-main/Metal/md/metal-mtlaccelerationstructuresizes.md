

- Metal
-  MTLAccelerationStructureSizes 

Structure

# MTLAccelerationStructureSizes

The expected sizes for a ray-tracing acceleration structure.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct MTLAccelerationStructureSizes
```

## Topics

### Retrieving the Sizes

var accelerationStructureSize: Int

The size of the acceleration structure, in bytes.

var buildScratchBufferSize: Int

The amount of scratch memory, in bytes, the GPU devices needs to build the acceleration structure.

var refitScratchBufferSize: Int

The amount of scratch memory, in bytes, the GPU device needs to refit the acceleration structure.

### Creating an Acceleration Size Structure

init()

Creates an acceleration sizes instance with default values.

init(accelerationStructureSize: Int, buildScratchBufferSize: Int, refitScratchBufferSize: Int)

Creates an acceleration sizes instance with specific values.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Creating Acceleration Structures for Ray Tracing

func makeAccelerationStructure(descriptor: MTLAccelerationStructureDescriptor) -> (any MTLAccelerationStructure)?

Creates a new ray-tracing acceleration structure from a descriptor.

**Required**

func makeAccelerationStructure(size: Int) -> (any MTLAccelerationStructure)?

Creates a new acceleration structure with a specific size.

**Required**

func accelerationStructureSizes(descriptor: MTLAccelerationStructureDescriptor) -> MTLAccelerationStructureSizes

Returns the buffer sizes the GPU device needs to build, refit, and store an acceleration structure.

**Required**

