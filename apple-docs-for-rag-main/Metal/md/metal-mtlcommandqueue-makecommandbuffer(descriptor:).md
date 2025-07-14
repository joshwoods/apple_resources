

- Metal
- MTLCommandQueue
-  makeCommandBuffer(descriptor:) 

Instance Method

# makeCommandBuffer(descriptor:)

Returns a command buffer from the command queue that you configure with a descriptor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func makeCommandBuffer(descriptor: MTLCommandBufferDescriptor) -> (any MTLCommandBuffer)?
```

**Required**

## Parameters 

`descriptor`  

An MTLCommandBufferDescriptor instance that configures the MTLCommandBuffer the method returns.

## Discussion

Use this method to create a command buffer that you configure with a descriptor. You can configure whether the command buffer retains references to resources that its commands refer to by setting the `descriptor` parameter’s retainedReferences property. You can also configure whether the command buffer saves extra error information, which is useful during development, by setting the descriptor’s errorOptions property.

Each command queue has a fixed number of command buffers for its lifetime (see makeCommandQueue(maxCommandBufferCount:)). This method blocks the calling CPU thread when the queue doesn’t have any free command buffers, and returns after the GPU finishes executing one.

## See Also

### Creating Command Buffers

func makeCommandBuffer() -> (any MTLCommandBuffer)?

Returns a command buffer from the command queue that maintains strong references to resources.

**Required**

func makeCommandBufferWithUnretainedReferences() -> (any MTLCommandBuffer)?

Returns a command buffer from the command queue that doesn’t maintain strong references to resources.

**Required**

