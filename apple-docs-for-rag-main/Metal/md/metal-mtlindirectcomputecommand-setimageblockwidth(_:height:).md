

- Metal
- MTLIndirectComputeCommand
-  setImageblockWidth(\_:height:) 

Instance Method

# setImageblockWidth(\_:height:)

Sets the size, in pixels, of the imageblock.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func setImageblockWidth(
    _ width: Int,
    height: Int
)
```

**Required**

## Parameters 

`width`  

The width of the imageblock.

`height`  

The height of the imageblock.

## See Also

### Setting a Command’s Arguments

func setComputePipelineState(any MTLComputePipelineState)

Sets the command’s compute pipeline state object.

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

