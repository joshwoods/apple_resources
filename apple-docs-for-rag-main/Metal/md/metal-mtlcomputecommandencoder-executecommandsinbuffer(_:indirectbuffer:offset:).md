

- Metal
- MTLComputeCommandEncoder
-  executeCommandsInBuffer(\_:indirectBuffer:offset:) 

Instance Method

# executeCommandsInBuffer(\_:indirectBuffer:offset:)

Encodes an instruction to run commands from an indirect buffer, using another buffer to provide the command range.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 13.0+visionOS

``` source
func executeCommandsInBuffer(
    _ buffer: any MTLIndirectCommandBuffer,
    indirectBuffer indirectRangeBuffer: any MTLBuffer,
    offset: Int
)
```

## Parameters 

`buffer`  

The MTLIndirectCommandBuffer instance containing the commands to execute.

`indirectRangeBuffer`  

An indirect buffer containing the execution range, laid out in an MTLIndirectCommandBufferExecutionRange instance. The maximum length of the range is `16384` commands.

`offset`  

The number of bytes from the start of `indirectRangeBuffer` containing the execution range to use. Align the offset on a multiple of `4`.

## See Also

### Dispatching from Indirect Command Buffers

func dispatchThreadgroups(indirectBuffer: any MTLBuffer, indirectBufferOffset: Int, threadsPerThreadgroup: MTLSize)

Encodes a dispatch call for a compute pass, using an indirect buffer that defines the size of a grid that aligns to threadgroup boundaries.

**Required**

func executeCommandsInBuffer(any MTLIndirectCommandBuffer, range: Range&lt;Int>)

Encodes an instruction to run commands from an indirect buffer.

func executeCommands(in: any MTLIndirectCommandBuffer, indirectBuffer: any MTLBuffer, indirectBufferOffset: Int)

Encodes an instruction to run commands from an indirect buffer, using another buffer to provide the command range.

func executeCommands(in: any MTLIndirectCommandBuffer, with: NSRange)

Encodes an instruction to run commands from an indirect buffer.

