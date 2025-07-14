

- Metal
- MTLComputeCommandEncoder
-  executeCommands(in:indirectBuffer:indirectBufferOffset:) 

Instance Method

# executeCommands(in:indirectBuffer:indirectBufferOffset:)

Encodes an instruction to run commands from an indirect buffer, using another buffer to provide the command range.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedmacOS 10.11+tvOS 13.0–14.0DeprecatedvisionOS

``` source
func executeCommands(
    in indirectCommandbuffer: any MTLIndirectCommandBuffer,
    indirectBuffer indirectRangeBuffer: any MTLBuffer,
    indirectBufferOffset: Int
)
```

## Parameters 

`indirectCommandbuffer`  

The MTLIndirectCommandBuffer instance containing the commands to execute.

`indirectRangeBuffer`  

An indirect buffer containing the execution range, laid out in an MTLIndirectCommandBufferExecutionRange instance. The maximum length of the range is `16384` commands.

`indirectBufferOffset`  

The number of bytes from the start of `indirectRangeBuffer` containing the execution range to use. Align the offset on a multiple of `4`.

## See Also

### Dispatching from Indirect Command Buffers

func dispatchThreadgroups(indirectBuffer: any MTLBuffer, indirectBufferOffset: Int, threadsPerThreadgroup: MTLSize)

Encodes a dispatch call for a compute pass, using an indirect buffer that defines the size of a grid that aligns to threadgroup boundaries.

**Required**

func executeCommandsInBuffer(any MTLIndirectCommandBuffer, range: Range&lt;Int>)

Encodes an instruction to run commands from an indirect buffer.

func executeCommandsInBuffer(any MTLIndirectCommandBuffer, indirectBuffer: any MTLBuffer, offset: Int)

Encodes an instruction to run commands from an indirect buffer, using another buffer to provide the command range.

func executeCommands(in: any MTLIndirectCommandBuffer, with: NSRange)

Encodes an instruction to run commands from an indirect buffer.

