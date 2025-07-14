

- Metal
- MTLComputeCommandEncoder
-  dispatchThreadgroups(indirectBuffer:indirectBufferOffset:threadsPerThreadgroup:) 

Instance Method

# dispatchThreadgroups(indirectBuffer:indirectBufferOffset:threadsPerThreadgroup:)

Encodes a dispatch call for a compute pass, using an indirect buffer that defines the size of a grid that aligns to threadgroup boundaries.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func dispatchThreadgroups(
    indirectBuffer: any MTLBuffer,
    indirectBufferOffset: Int,
    threadsPerThreadgroup: MTLSize
)
```

**Required**

## Parameters 

`indirectBuffer`  

An MTLBuffer instance providing compute parameters. Lay out the data in this buffer as described in the MTLDispatchThreadgroupsIndirectArguments structure.

`indirectBufferOffset`  

Where the data begins, in bytes, from the start of the buffer. This value must be a multiple of `4`.

`threadsPerThreadgroup`  

The number of threads in one threadgroup, in each dimension.

## Discussion

The GPU fetches parameters from the indirect buffer just before the thread grid starts. This process lets the compute function run based on GPU feedback, without latency from data transfer between the CPU and the GPU.

## See Also

### Dispatching from Indirect Command Buffers

func executeCommandsInBuffer(any MTLIndirectCommandBuffer, range: Range&lt;Int>)

Encodes an instruction to run commands from an indirect buffer.

func executeCommandsInBuffer(any MTLIndirectCommandBuffer, indirectBuffer: any MTLBuffer, offset: Int)

Encodes an instruction to run commands from an indirect buffer, using another buffer to provide the command range.

func executeCommands(in: any MTLIndirectCommandBuffer, indirectBuffer: any MTLBuffer, indirectBufferOffset: Int)

Encodes an instruction to run commands from an indirect buffer, using another buffer to provide the command range.

func executeCommands(in: any MTLIndirectCommandBuffer, with: NSRange)

Encodes an instruction to run commands from an indirect buffer.

