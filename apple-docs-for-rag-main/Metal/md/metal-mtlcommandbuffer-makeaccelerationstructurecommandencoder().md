

- Metal
- MTLCommandBuffer
-  makeAccelerationStructureCommandEncoder() 

Instance Method

# makeAccelerationStructureCommandEncoder()

Creates a ray-tracing acceleration structure command encoder that uses default settings.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func makeAccelerationStructureCommandEncoder() -> (any MTLAccelerationStructureCommandEncoder)?
```

**Required**

## Discussion

Use an MTLAccelerationStructureCommandEncoder instance’s methods to set up a single ray-tracing pass.

## See Also

### Creating Acceleration Structure Encoders

func makeAccelerationStructureCommandEncoder(descriptor: MTLAccelerationStructurePassDescriptor) -> any MTLAccelerationStructureCommandEncoder

Creates a ray-tracing acceleration structure command encoder from a descriptor.

**Required**

