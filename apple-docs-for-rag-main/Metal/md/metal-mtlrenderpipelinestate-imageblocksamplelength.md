

- Metal
- MTLRenderPipelineState
-  imageblockSampleLength 

Instance Property

# imageblockSampleLength

The memory size, in byes, of the render pipeline’s imageblock for a single sample.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
var imageblockSampleLength: Int { get }
```

**Required**

## See Also

### Checking Tile Shader Memory Requirements

var maxTotalThreadsPerThreadgroup: Int

The largest number of threads the pipeline state can have in a single tile shader threadgroup.

**Required**

var threadgroupSizeMatchesTileSize: Bool

A Boolean value that indicates whether the pipeline state needs a threadgroup’s size to equal a tile’s size.

**Required**

func imageblockMemoryLength(forDimensions: MTLSize) -> Int

Returns the length of an imageblock’s memory for the specified imageblock dimensions.

**Required**

