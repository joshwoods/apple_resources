

- Metal
- MTLIOCommandQueue
-  makeCommandBuffer() 

Instance Method

# makeCommandBuffer()

Creates an input/output command buffer for the command queue.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func makeCommandBuffer() -> any MTLIOCommandBuffer
```

**Required**

## See Also

### Creating a Input/Output Command Buffer

func makeCommandBufferWithUnretainedReferences() -> any MTLIOCommandBuffer

Creates an input/output command buffer for the command queue that doesn’t retain the instances you pass to its methods.

**Required**

