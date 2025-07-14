

- Metal
- MTLRenderPipelineState
-  imageblockMemoryLength(forDimensions:) 

Instance Method

# imageblockMemoryLength(forDimensions:)

Returns the length of an imageblock’s memory for the specified imageblock dimensions.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
func imageblockMemoryLength(forDimensions imageblockDimensions: MTLSize) -> Int
```

**Required**

## Parameters 

`imageblockDimensions`  

An MTLSize instance that represent the dimensions of an imageblock.

## Discussion

The imageblock dimensions must match a valid tile size, such as one of the following:

- 32 x 32

- 32 x 16

- 16 x 16

The GPU partitions tile memory between imageblocks and threadgroup memory,

Important

The total memory allocations for imageblocks and threadgroup memory can’t exceed the tile memory limit for the GPU device.

For information about identifying tile memory limits for GPU devices, see either of the following:

- Metal Feature Set Tables (PDF)

- Metal Feature Set Tables (Numbers)

## See Also

### Checking Tile Shader Memory Requirements

var maxTotalThreadsPerThreadgroup: Int

The largest number of threads the pipeline state can have in a single tile shader threadgroup.

**Required**

var threadgroupSizeMatchesTileSize: Bool

A Boolean value that indicates whether the pipeline state needs a threadgroup’s size to equal a tile’s size.

**Required**

var imageblockSampleLength: Int

The memory size, in byes, of the render pipeline’s imageblock for a single sample.

**Required**

