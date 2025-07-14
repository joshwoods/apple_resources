

- Metal
- MTLCommandBuffer
-  makeComputeCommandEncoder(dispatchType:) 

Instance Method

# makeComputeCommandEncoder(dispatchType:)

Creates a compute command encoder with a dispatch type.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func makeComputeCommandEncoder(dispatchType: MTLDispatchType) -> (any MTLComputeCommandEncoder)?
```

**Required**

## Parameters 

`dispatchType`  

An MTLDispatchType instance that indicates whether the compute pass the encoder creates runs commands serially or concurrently.

## Discussion

Use an MTLComputeCommandEncoder instance’s methods to set up a single compute pass.

## See Also

### Creating Compute Encoders

func makeComputeCommandEncoder(descriptor: MTLComputePassDescriptor) -> (any MTLComputeCommandEncoder)?

Creates a compute command encoder from a descriptor.

**Required**

func makeComputeCommandEncoder() -> (any MTLComputeCommandEncoder)?

Creates a compute command encoder that uses default settings.

**Required**

enum MTLDispatchType

The type of dispatch method to use when calling encoded functions.

