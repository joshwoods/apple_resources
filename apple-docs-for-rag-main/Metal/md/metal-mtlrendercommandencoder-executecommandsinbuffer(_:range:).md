

- Metal
- MTLRenderCommandEncoder
-  executeCommandsInBuffer(\_:range:) 

Instance Method

# executeCommandsInBuffer(\_:range:)

Encodes a command that runs a range of commands from an indirect command buffer (ICB).

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.14+tvOS 12.0+visionOS

``` source
func executeCommandsInBuffer(
    _ buffer: any MTLIndirectCommandBuffer,
    range: Range
)
```

## Parameters 

`buffer`  

An MTLIndirectCommandBuffer instance that contains other commands the current command runs.

`range`  

A span of integers that represent the command entries in `buffer` the current command runs. The number of commands needs to be less than or equal to `0x4000` (`16,384`).

## See Also

### Encoding Commands that Run Indirect Command Buffers

func executeCommandsInBuffer(any MTLIndirectCommandBuffer, indirectBuffer: any MTLBuffer, offset: Int)

Encodes a command that runs an indirect range of commands from an indirect command buffer (ICB).

