

- MetalKit
- MTKTextureLoader
- MTKTextureLoader.Origin
-  bottomLeft 

Type Property

# bottomLeft

An option for specifying images that should be flipped only to put their origin in the bottom-left corner.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
static let bottomLeft: MTKTextureLoader.Origin
```

## Discussion

The texture will be flipped vertically if metadata in the file being loaded indicates that the source data starts with the top-left corner of the texture.

## See Also

### Specifying Texture Origin Options

static let topLeft: MTKTextureLoader.Origin

An option for specifying images that should be flipped only to put their origin in the top-left corner.

static let flippedVertically: MTKTextureLoader.Origin

An option that specifies that images should always be flipped.

