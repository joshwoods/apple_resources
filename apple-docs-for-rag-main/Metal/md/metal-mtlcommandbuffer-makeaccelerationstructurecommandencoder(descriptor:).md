

- Metal
- MTLCommandBuffer
-  makeAccelerationStructureCommandEncoder(descriptor:) 

Instance Method

# makeAccelerationStructureCommandEncoder(descriptor:)

Creates a ray-tracing acceleration structure command encoder from a descriptor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func makeAccelerationStructureCommandEncoder(descriptor: MTLAccelerationStructurePassDescriptor) -> any MTLAccelerationStructureCommandEncoder
```

**Required**

## Parameters 

`descriptor`  

An MTLAccelerationStructurePassDescriptor instance that configures the MTLAccelerationStructureCommandEncoder the method returns.

## Discussion

Use an MTLAccelerationStructureCommandEncoder instance’s methods to set up a single ray-tracing pass.

## See Also

### Creating Acceleration Structure Encoders

func makeAccelerationStructureCommandEncoder() -> (any MTLAccelerationStructureCommandEncoder)?

Creates a ray-tracing acceleration structure command encoder that uses default settings.

**Required**

