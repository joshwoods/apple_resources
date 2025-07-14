

- Metal
- MTLRenderCommandEncoder
-  tileWidth 

Instance Property

# tileWidth

The width of the tiles, in pixels, for the render command encoder.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
var tileWidth: Int { get }
```

**Required**

## Discussion

The value comes from the tileWidth property of the MTLRenderPassDescriptor at the time you create the render command encoder.

## See Also

### Drawing with Tile Shaders

func dispatchThreadsPerTile(MTLSize)

Encodes a command that invokes GPU functions from the encoder’s current tile render pipeline state.

**Required**

var tileHeight: Int

The height of the tiles, in pixels, for the render command encoder.

**Required**

