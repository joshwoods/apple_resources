

- Metal
- MTLComputeCommandEncoder
-  setStageInRegionWithIndirectBuffer(\_:indirectBufferOffset:) 

Instance Method

# setStageInRegionWithIndirectBuffer(\_:indirectBufferOffset:)

Sets the region of the stage-in attributes to apply to a compute kernel using an indirect buffer.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func setStageInRegionWithIndirectBuffer(
    _ indirectBuffer: any MTLBuffer,
    indirectBufferOffset: Int
)
```

**Required**

## Parameters 

`indirectBuffer`  

The MTLRegion defining how to interpret a thread’s location as a coordinate for stage-in data.

`indirectBufferOffset`  

Where the data begins, in bytes, from the start of the buffer.

## Discussion

Important

Lay out the data in the buffer as described in the MTLStageInRegionIndirectArguments structure.

The region’s origin point, starting from `(0,0,0)` in the upper left of the bound data, determines the final index of `[[stage_in]]` data. Note that the total number of threads Metal launches may be larger than your stage-in data.

To determine the index used to fetch `[[stage_in]]` data for a given thread, the GPU adds the values specified by the region’s origin to the thread position in the grid. Threads in the grid outside of the maximum stage-in data size have undefined behavior when accessing the stage-in memory region.

## See Also

### Encoding Stage-in Data

func setStageInRegion(MTLRegion)

Sets the dimensions over the thread grid of how your compute kernel receives stage-in arguments.

**Required**

