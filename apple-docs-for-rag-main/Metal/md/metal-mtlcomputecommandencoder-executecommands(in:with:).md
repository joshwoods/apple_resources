

- Metal
- MTLComputeCommandEncoder
-  executeCommands(in:with:) 

Instance Method

# executeCommands(in:with:)

Encodes an instruction to run commands from an indirect buffer.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedmacOS 10.11+tvOS 13.0–14.0DeprecatedvisionOS

``` source
func executeCommands(
    in indirectCommandBuffer: any MTLIndirectCommandBuffer,
    with executionRange: NSRange
)
```

## Parameters 

`indirectCommandBuffer`  

The MTLIndirectCommandBuffer instance containing the commands to execute.

`executionRange`  

The range of commands to execute. The maximum length of the range is `16384` commands.

## See Also

### Dispatching from Indirect Command Buffers

func dispatchThreadgroups(indirectBuffer: any MTLBuffer, indirectBufferOffset: Int, threadsPerThreadgroup: MTLSize)

Encodes a dispatch call for a compute pass, using an indirect buffer that defines the size of a grid that aligns to threadgroup boundaries.

**Required**

func executeCommandsInBuffer(any MTLIndirectCommandBuffer, range: Range&lt;Int>)

Encodes an instruction to run commands from an indirect buffer.

func executeCommandsInBuffer(any MTLIndirectCommandBuffer, indirectBuffer: any MTLBuffer, offset: Int)

Encodes an instruction to run commands from an indirect buffer, using another buffer to provide the command range.

func executeCommands(in: any MTLIndirectCommandBuffer, indirectBuffer: any MTLBuffer, indirectBufferOffset: Int)

Encodes an instruction to run commands from an indirect buffer, using another buffer to provide the command range.

