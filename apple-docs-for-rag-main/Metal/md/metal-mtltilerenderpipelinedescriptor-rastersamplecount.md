

- Metal
- MTLTileRenderPipelineDescriptor
-  rasterSampleCount 

Instance Property

# rasterSampleCount

The number of samples in each fragment.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
var rasterSampleCount: Int { get set }
```

## Discussion

The default value is `1`. This value is used only if the pipeline render targets support multisampling. If the render targets don’t support multisampling, then this value must be `1`.

When you create a MTLRenderCommandEncoder, the sampleCount value of all attachments must match this `sampleCount` value. Furthermore, the texture type of all attachments must be MTLTextureType.type2DMultisample.

Support for different sample count values varies by device object. Call the supportsTextureSampleCount(_:) method on a MTLDevice object to determine whether it supports a specific sample count.

## See Also

### Specifying Rasterization and Visibility State

var threadgroupSizeMatchesTileSize: Bool

A Boolean value that indicates whether all threadgroups for this pipeline completely cover tiles.

