

- Metal
- MTLIndirectComputeCommand
-  setComputePipelineState(\_:) 

Instance Method

# setComputePipelineState(\_:)

Sets the command’s compute pipeline state object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 11.0+tvOS 13.0+visionOS 1.0+

``` source
func setComputePipelineState(_ pipelineState: any MTLComputePipelineState)
```

**Required**

## Parameters 

`pipelineState`  

The compute pipeline state object to use.

## Discussion

If you created the indirect command buffer with inheritPipelineState set to true, do not call this method. The command gets the pipeline state object from the parent encoder when you execute the command.

If you created the indirect command buffer with inheritPipelineState set to false, you must set the pipeline state prior to encoding the drawing command.

## See Also

### Setting a Command’s Arguments

func setImageblockWidth(Int, height: Int)

Sets the size, in pixels, of the imageblock.

**Required**

func setKernelBuffer(any MTLBuffer, offset: Int, at: Int)

Sets a buffer for the compute function.

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

