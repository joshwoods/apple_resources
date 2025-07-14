

- Metal
- MTLRenderPassDescriptor
-  imageblockSampleLength 

Instance Property

# imageblockSampleLength

The per-sample size, in bytes, of the largest explicit imageblock layout in the render pass.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
var imageblockSampleLength: Int { get set }
```

## Discussion

If `imageBlockSampleLength` isn’t specified, Metal determines the imageblock sample length from the render pass attachment formats. If any render pipelines bound to the encoder reference imageblocks with explicit layout, you must set this property.

## See Also

### Specifying Tile Shading Parameters

var threadgroupMemoryLength: Int

The per-tile size, in bytes, of the persistent threadgroup memory allocation.

var tileWidth: Int

The tile width, in pixels.

var tileHeight: Int

The tile height, in pixels.

