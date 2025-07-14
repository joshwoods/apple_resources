

- Metal
- MTLIOCommandQueue
-  makeCommandBufferWithUnretainedReferences() 

Instance Method

# makeCommandBufferWithUnretainedReferences()

Creates an input/output command buffer for the command queue that doesn’t retain the instances you pass to its methods.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func makeCommandBufferWithUnretainedReferences() -> any MTLIOCommandBuffer
```

**Required**

## See Also

### Creating a Input/Output Command Buffer

func makeCommandBuffer() -> any MTLIOCommandBuffer

Creates an input/output command buffer for the command queue.

**Required**

