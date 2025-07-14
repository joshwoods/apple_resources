

- Metal
- MTLIndirectComputeCommand
-  setStageIn(\_:) 

Instance Method

# setStageIn(\_:)

Sets the region of the stage-in attributes to apply to the compute kernel.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedMac Catalyst 14.0–14.0DeprecatedtvOS 13.0–14.0DeprecatedvisionOS

``` source
func setStageIn(_ region: MTLRegion)
```

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

func setStageInRegion(MTLRegion)

Sets the region of the stage-in attributes to apply to the compute kernel.

**Required**

