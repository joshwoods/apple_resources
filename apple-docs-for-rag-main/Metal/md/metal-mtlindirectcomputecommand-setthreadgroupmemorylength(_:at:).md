

- Metal
- MTLIndirectComputeCommand
-  setThreadgroupMemoryLength(\_:at:) 

Instance Method

# setThreadgroupMemoryLength(\_:at:)

Sets the size of a block of threadgroup memory.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedMac Catalyst 14.0–14.0DeprecatedtvOS 13.0–14.0DeprecatedvisionOS

``` source
func setThreadgroupMemoryLength(
    _ length: Int,
    at index: Int
)
```

## Parameters 

`length`  

The size of the threadgroup memory, in bytes. Must be a multiple of 16 bytes.

`index`  

The index in the threadgroup memory argument table.

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

func setStageInRegion(MTLRegion)

Sets the region of the stage-in attributes to apply to the compute kernel.

**Required**

func setStageIn(MTLRegion)

Sets the region of the stage-in attributes to apply to the compute kernel.

