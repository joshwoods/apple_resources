

- Metal
- MTLDevice
-  accelerationStructureSizes(descriptor:) 

Instance Method

# accelerationStructureSizes(descriptor:)

Returns the buffer sizes the GPU device needs to build, refit, and store an acceleration structure.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func accelerationStructureSizes(descriptor: MTLAccelerationStructureDescriptor) -> MTLAccelerationStructureSizes
```

**Required**

## Parameters 

`descriptor`  

An MTLAccelerationStructureDescriptor instance.

## Return Value

A new MTLAccelerationStructureSizes instance.

## See Also

### Creating Acceleration Structures for Ray Tracing

func makeAccelerationStructure(descriptor: MTLAccelerationStructureDescriptor) -> (any MTLAccelerationStructure)?

Creates a new ray-tracing acceleration structure from a descriptor.

**Required**

func makeAccelerationStructure(size: Int) -> (any MTLAccelerationStructure)?

Creates a new acceleration structure with a specific size.

**Required**

struct MTLAccelerationStructureSizes

The expected sizes for a ray-tracing acceleration structure.

