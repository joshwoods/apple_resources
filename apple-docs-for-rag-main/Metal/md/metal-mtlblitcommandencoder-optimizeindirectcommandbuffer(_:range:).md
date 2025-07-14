

- Metal
- MTLBlitCommandEncoder
-  optimizeIndirectCommandBuffer(\_:range:) 

Instance Method

# optimizeIndirectCommandBuffer(\_:range:)

Encodes a command that can improve the performance of a range of commands within an indirect command buffer.

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.14+tvOS 12.0+visionOS

``` source
func optimizeIndirectCommandBuffer(
    _ buffer: any MTLIndirectCommandBuffer,
    range: Range
)
```

## Parameters 

`buffer`  

An indirect command buffer the command optimizes.

`range`  

A range of commands within `indirectCommandBuffer`.

## Discussion

This command can reduce the time it takes the GPU to run the commands within an indirect command buffer by removing its redundancies. For example, an indirect command buffer may have empty commands or commands that duplicate identical state. Redundancies like these can come from multiple compute functions that encode commands in parallel, which can sometimes reset commands or configure identical states multiple times.

Important

You can only run optimized commands by using the entire range. Otherwise, starting or ending within an optimized range may result in unexpected behavior.

You can’t run any commands that start or end at an index within that range, or that cross into another optimized range. However, you can reuse the range you optimize by resetting it and then encoding new commands to it.

## See Also

### Working with Indirect Command Buffers

func copyIndirectCommandBuffer(any MTLIndirectCommandBuffer, sourceRange: Range&lt;Int>, destination: any MTLIndirectCommandBuffer, destinationIndex: Int)

Encodes a command that copies commands from one indirect command buffer into another.

func resetCommandsInBuffer(any MTLIndirectCommandBuffer, range: Range&lt;Int>)

Encodes a command that resets a range of commands in an indirect command buffer.

