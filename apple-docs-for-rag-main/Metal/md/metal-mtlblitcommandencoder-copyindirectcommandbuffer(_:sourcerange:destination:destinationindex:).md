

- Metal
- MTLBlitCommandEncoder
-  copyIndirectCommandBuffer(\_:sourceRange:destination:destinationIndex:) 

Instance Method

# copyIndirectCommandBuffer(\_:sourceRange:destination:destinationIndex:)

Encodes a command that copies commands from one indirect command buffer into another.

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.14+tvOS 12.0+visionOS

``` source
func copyIndirectCommandBuffer(
    _ buffer: any MTLIndirectCommandBuffer,
    sourceRange: Range,
    destination: any MTLIndirectCommandBuffer,
    destinationIndex: Int
)
```

## Parameters 

`buffer`  

An indirect command buffer the command copies from.

`sourceRange`  

The range of commands in the source buffer to copy. The source range needs to start on a valid execution point.

`destination`  

Another indirect command buffer the command copies to.

`destinationIndex`  

An index in `destination` where the command copies content from `source` to. The destination index needs to be a valid execution point with enough remaining space in `destination` to accommodate `sourceRange.count` indexes.

## Discussion

You can copy commands from one indirect command buffer to another, but only a compatible one. You can create compatible indirect command buffers by passing MTLIndirectCommandBufferDescriptor instances with the same configuration to the makeIndirectCommandBuffer(descriptor:maxCommandCount:options:) method of MTLDevice.

## See Also

### Working with Indirect Command Buffers

func resetCommandsInBuffer(any MTLIndirectCommandBuffer, range: Range&lt;Int>)

Encodes a command that resets a range of commands in an indirect command buffer.

func optimizeIndirectCommandBuffer(any MTLIndirectCommandBuffer, range: Range&lt;Int>)

Encodes a command that can improve the performance of a range of commands within an indirect command buffer.

