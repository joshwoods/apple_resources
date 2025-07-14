

- Metal
- MTLIOCommandBuffer
-  copyStatus(buffer:offset:) 

Instance Method

# copyStatus(buffer:offset:)

Encodes a command that writes the input/output command buffer’s status to a buffer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func copyStatus(
    buffer: any MTLBuffer,
    offset: Int
)
```

**Required**

## Parameters 

`buffer`  

A buffer instance the method copies the status into.

`offset`  

A starting location relative to the beginning of the buffer, in bytes, the method copies data to.

## See Also

### Adding Final Commands

func addCompletedHandler(MTLIOCommandBufferHandler)

Adds a closure that Metal calls immediately after the GPU finishes executing the commands in the input/output command buffer.

**Required**

