

- Metal
- MTLCommandBuffer
-  makeComputeCommandEncoder() 

Instance Method

# makeComputeCommandEncoder()

Creates a compute command encoder that uses default settings.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeComputeCommandEncoder() -> (any MTLComputeCommandEncoder)?
```

**Required**

## Discussion

Use an MTLComputeCommandEncoder instance’s methods to set up a single compute pass. The encoder this method returns dispatches its compute commands serially (see MTLDispatchType.serial). To create a compute command encoder that dispatches commands concurrently (see MTLDispatchType.concurrent), use the makeComputeCommandEncoder(dispatchType:) or makeComputeCommandEncoder(descriptor:) method.

## See Also

### Creating Compute Encoders

func makeComputeCommandEncoder(descriptor: MTLComputePassDescriptor) -> (any MTLComputeCommandEncoder)?

Creates a compute command encoder from a descriptor.

**Required**

func makeComputeCommandEncoder(dispatchType: MTLDispatchType) -> (any MTLComputeCommandEncoder)?

Creates a compute command encoder with a dispatch type.

**Required**

enum MTLDispatchType

The type of dispatch method to use when calling encoded functions.

