

- Metal
- MTLRenderCommandEncoder
-  executeCommandsInBuffer(\_:indirectBuffer:offset:) 

Instance Method

# executeCommandsInBuffer(\_:indirectBuffer:offset:)

Encodes a command that runs an indirect range of commands from an indirect command buffer (ICB).

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.14+tvOS 13.0+visionOS

``` source
func executeCommandsInBuffer(
    _ buffer: any MTLIndirectCommandBuffer,
    indirectBuffer indirectRangeBuffer: any MTLBuffer,
    offset: Int
)
```

## Parameters 

`buffer`  

An MTLIndirectCommandBuffer instance that contains other commands the current command runs.

`indirectRangeBuffer`  

An MTLBuffer instance with data that matches the layout of the MTLIndirectCommandBufferExecutionRange structure.

The length property of that structure needs to be less than or equal to `0x4000` (`16,384`).

`offset`  

An integer that represents the location, in bytes, from the start of `indirectRangeBuffer` where the execution range structure begins.

See the Metal feature set tables (PDF) to check for offset alignment requirements for buffers in `device` and `constant` address space.

## See Also

### Encoding Commands that Run Indirect Command Buffers

func executeCommandsInBuffer(any MTLIndirectCommandBuffer, range: Range&lt;Int>)

Encodes a command that runs a range of commands from an indirect command buffer (ICB).

