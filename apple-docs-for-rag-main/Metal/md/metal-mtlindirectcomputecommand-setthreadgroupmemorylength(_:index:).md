

- Metal
- MTLIndirectComputeCommand
-  setThreadgroupMemoryLength(\_:index:) 

Instance Method

# setThreadgroupMemoryLength(\_:index:)

Sets the size of a block of threadgroup memory.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 11.0+tvOS 13.0+visionOS 1.0+

``` source
func setThreadgroupMemoryLength(
    _ length: Int,
    index: Int
)
```

**Required**

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

func setThreadgroupMemoryLength(Int, at: Int)

Sets the size of a block of threadgroup memory.

func setStageInRegion(MTLRegion)

Sets the region of the stage-in attributes to apply to the compute kernel.

**Required**

func setStageIn(MTLRegion)

Sets the region of the stage-in attributes to apply to the compute kernel.

