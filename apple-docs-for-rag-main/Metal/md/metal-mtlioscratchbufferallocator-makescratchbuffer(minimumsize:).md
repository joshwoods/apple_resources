

- Metal
- MTLIOScratchBufferAllocator
-  makeScratchBuffer(minimumSize:) 

Instance Method

# makeScratchBuffer(minimumSize:)

Creates a scratch memory buffer for an input/output command queue.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func makeScratchBuffer(minimumSize: Int) -> (any MTLIOScratchBuffer)?
```

**Required**

## Parameters 

`minimumSize`  

The number of bytes the input/output command buffer needs to successfully run a command buffer.

## Return Value

A MTLIOScratchBuffer instance that your app implements or `nil`.

## Discussion

Your app can reduce additional callbacks from the framework by providing additional memory above `minimumSize`. If your implementation returns `nil`, the input/output command queue cancels the MTLIOCommandBuffer instance that needs the scratch buffer memory.

