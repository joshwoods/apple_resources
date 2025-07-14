

- Metal
- MTLBlitCommandEncoder
-  resetCommandsInBuffer(\_:range:) 

Instance Method

# resetCommandsInBuffer(\_:range:)

Encodes a command that resets a range of commands in an indirect command buffer.

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.14+tvOS 12.0+visionOS

``` source
func resetCommandsInBuffer(
    _ buffer: any MTLIndirectCommandBuffer,
    range: Range
)
```

## Parameters 

`buffer`  

An indirect command buffer the command resets.

`range`  

A range of commands within `buffer`.

## See Also

### Working with Indirect Command Buffers

func copyIndirectCommandBuffer(any MTLIndirectCommandBuffer, sourceRange: Range&lt;Int>, destination: any MTLIndirectCommandBuffer, destinationIndex: Int)

Encodes a command that copies commands from one indirect command buffer into another.

func optimizeIndirectCommandBuffer(any MTLIndirectCommandBuffer, range: Range&lt;Int>)

Encodes a command that can improve the performance of a range of commands within an indirect command buffer.

