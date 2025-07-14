

- Metal
- MTLComputeCommandEncoder
-  executeCommandsInBuffer(\_:range:) 

Instance Method

# executeCommandsInBuffer(\_:range:)

Encodes an instruction to run commands from an indirect buffer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 13.0+visionOS

``` source
func executeCommandsInBuffer(
    _ buffer: any MTLIndirectCommandBuffer,
    range: Range
)
```

## Parameters 

`buffer`  

The MTLIndirectCommandBuffer instance containing the commands to execute.

`range`  

The range of commands to execute. The maximum length of the range is `16384` commands.

## See Also

### Dispatching from Indirect Command Buffers

func dispatchThreadgroups(indirectBuffer: any MTLBuffer, indirectBufferOffset: Int, threadsPerThreadgroup: MTLSize)

Encodes a dispatch call for a compute pass, using an indirect buffer that defines the size of a grid that aligns to threadgroup boundaries.

**Required**

func executeCommandsInBuffer(any MTLIndirectCommandBuffer, indirectBuffer: any MTLBuffer, offset: Int)

Encodes an instruction to run commands from an indirect buffer, using another buffer to provide the command range.

func executeCommands(in: any MTLIndirectCommandBuffer, indirectBuffer: any MTLBuffer, indirectBufferOffset: Int)

Encodes an instruction to run commands from an indirect buffer, using another buffer to provide the command range.

func executeCommands(in: any MTLIndirectCommandBuffer, with: NSRange)

Encodes an instruction to run commands from an indirect buffer.

