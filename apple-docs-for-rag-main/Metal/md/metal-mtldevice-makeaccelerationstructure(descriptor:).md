

- Metal
- MTLDevice
-  makeAccelerationStructure(descriptor:) 

Instance Method

# makeAccelerationStructure(descriptor:)

Creates a new ray-tracing acceleration structure from a descriptor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func makeAccelerationStructure(descriptor: MTLAccelerationStructureDescriptor) -> (any MTLAccelerationStructure)?
```

**Required**

## Parameters 

`descriptor`  

An MTLAccelerationStructureDescriptor instance.

## Return Value

A new MTLAccelerationStructure instance if the method completed successfully; otherwise `nil`.

## See Also

### Creating Acceleration Structures for Ray Tracing

func makeAccelerationStructure(size: Int) -> (any MTLAccelerationStructure)?

Creates a new acceleration structure with a specific size.

**Required**

func accelerationStructureSizes(descriptor: MTLAccelerationStructureDescriptor) -> MTLAccelerationStructureSizes

Returns the buffer sizes the GPU device needs to build, refit, and store an acceleration structure.

**Required**

struct MTLAccelerationStructureSizes

The expected sizes for a ray-tracing acceleration structure.

