

- Metal
- MTLIndirectComputeCommand
-  setStageInRegion(\_:) 

Instance Method

# setStageInRegion(\_:)

Sets the region of the stage-in attributes to apply to the compute kernel.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 11.0+tvOS 13.0+visionOS 1.0+

``` source
func setStageInRegion(_ region: MTLRegion)
```

**Required**

## Parameters 

`region`  

The offset and maximum size of the grid over which compute threads that read per-thread stage-in data are launched.

## See Also

### Setting a Command’s Arguments

func setComputePipelineState(any MTLComputePipelineState)

Sets the command’s compute pipeline state object.

**Required**

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

func setStageIn(MTLRegion)

Sets the region of the stage-in attributes to apply to the compute kernel.

