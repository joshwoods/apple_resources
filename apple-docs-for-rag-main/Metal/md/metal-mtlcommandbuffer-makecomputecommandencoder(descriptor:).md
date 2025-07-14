

- Metal
- MTLCommandBuffer
-  makeComputeCommandEncoder(descriptor:) 

Instance Method

# makeComputeCommandEncoder(descriptor:)

Creates a compute command encoder from a descriptor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func makeComputeCommandEncoder(descriptor computePassDescriptor: MTLComputePassDescriptor) -> (any MTLComputeCommandEncoder)?
```

**Required**

## Parameters 

`computePassDescriptor`  

An MTLComputePassDescriptor instance that configures the MTLComputeCommandEncoder the method returns.

## Discussion

Use an MTLComputeCommandEncoder instance’s methods to set up a single compute pass.

## See Also

### Creating Compute Encoders

func makeComputeCommandEncoder() -> (any MTLComputeCommandEncoder)?

Creates a compute command encoder that uses default settings.

**Required**

func makeComputeCommandEncoder(dispatchType: MTLDispatchType) -> (any MTLComputeCommandEncoder)?

Creates a compute command encoder with a dispatch type.

**Required**

enum MTLDispatchType

The type of dispatch method to use when calling encoded functions.

