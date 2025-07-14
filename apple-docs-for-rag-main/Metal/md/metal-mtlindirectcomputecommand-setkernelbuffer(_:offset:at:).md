

- Metal
- MTLIndirectComputeCommand
-  setKernelBuffer(\_:offset:at:) 

Instance Method

# setKernelBuffer(\_:offset:at:)

Sets a buffer for the compute function.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 11.0+tvOS 13.0+visionOS 1.0+

``` source
func setKernelBuffer(
    _ buffer: any MTLBuffer,
    offset: Int,
    at index: Int
)
```

**Required**

## Parameters 

`buffer`  

The buffer to set in the buffer argument table.

`offset`  

Where the data begins, in bytes, from the start of the buffer.

`index`  

An index in the buffer argument table.

## Discussion

If you created the indirect command buffer with inheritBuffers set to true, don’t call this method. The command gets the arguments from the parent encoder when you execute the command.

If you need to pass other kinds of parameters to your shader, such as textures and samplers, create an argument buffer and pass it to the shader using this method.

## See Also

### Setting a Command’s Arguments

func setComputePipelineState(any MTLComputePipelineState)

Sets the command’s compute pipeline state object.

**Required**

func setImageblockWidth(Int, height: Int)

Sets the size, in pixels, of the imageblock.

**Required**

func setThreadgroupMemoryLength(Int, index: Int)

Sets the size of a block of threadgroup memory.

**Required**

func setThreadgroupMemoryLength(Int, at: Int)

Sets the size of a block of threadgroup memory.

func setStageInRegion(MTLRegion)

Sets the region of the stage-in attributes to apply to the compute kernel.

**Required**

func setStageIn(MTLRegion)

Sets the region of the stage-in attributes to apply to the compute kernel.

