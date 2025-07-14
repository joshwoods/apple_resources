

- Metal
- MTLCommandQueue
-  makeCommandBuffer() 

Instance Method

# makeCommandBuffer()

Returns a command buffer from the command queue that maintains strong references to resources.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeCommandBuffer() -> (any MTLCommandBuffer)?
```

**Required**

## Mentioned in 

Setting Up a Command Structure

## Discussion

The command buffers you create with this method maintain strong references to the resources you encode into it, including buffers, textures, samplers, and pipeline states. The command buffer releases these references after it finishes running on the GPU.

This method sets the retainedReferences property to true for the command buffer it creates.

Each command queue has a fixed number of command buffers for its lifetime (see makeCommandQueue(maxCommandBufferCount:)). This method blocks the calling CPU thread when the queue doesn’t have any free command buffers, and returns after the GPU finishes executing one.

## See Also

### Creating Command Buffers

func makeCommandBuffer(descriptor: MTLCommandBufferDescriptor) -> (any MTLCommandBuffer)?

Returns a command buffer from the command queue that you configure with a descriptor.

**Required**

func makeCommandBufferWithUnretainedReferences() -> (any MTLCommandBuffer)?

Returns a command buffer from the command queue that doesn’t maintain strong references to resources.

**Required**

