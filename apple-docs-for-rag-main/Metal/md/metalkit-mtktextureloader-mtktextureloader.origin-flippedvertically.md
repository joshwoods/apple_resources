

- MetalKit
- MTKTextureLoader
- MTKTextureLoader.Origin
-  flippedVertically 

Type Property

# flippedVertically

An option that specifies that images should always be flipped.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
static let flippedVertically: MTKTextureLoader.Origin
```

## Discussion

The texture will be flipped vertically regardless of any metadata in the file indicating the placement of the origin in the source data.

## See Also

### Specifying Texture Origin Options

static let topLeft: MTKTextureLoader.Origin

An option for specifying images that should be flipped only to put their origin in the top-left corner.

static let bottomLeft: MTKTextureLoader.Origin

An option for specifying images that should be flipped only to put their origin in the bottom-left corner.

