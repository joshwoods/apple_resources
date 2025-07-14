

- Metal
- MTLTileRenderPipelineDescriptor
-  threadgroupSizeMatchesTileSize 

Instance Property

# threadgroupSizeMatchesTileSize

A Boolean value that indicates whether all threadgroups for this pipeline completely cover tiles.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
var threadgroupSizeMatchesTileSize: Bool { get set }
```

## Discussion

Metal can optimize code generation when the threadgroup and tile sizes match.

## See Also

### Specifying Rasterization and Visibility State

var rasterSampleCount: Int

The number of samples in each fragment.

