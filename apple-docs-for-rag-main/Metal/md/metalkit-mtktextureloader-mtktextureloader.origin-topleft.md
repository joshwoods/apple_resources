

- MetalKit
- MTKTextureLoader
- MTKTextureLoader.Origin
-  topLeft 

Type Property

# topLeft

An option for specifying images that should be flipped only to put their origin in the top-left corner.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
static let topLeft: MTKTextureLoader.Origin
```

## Discussion

The texture will be flipped vertically if metadata in the file being loaded indicates that the source data starts with the bottom-left corner of the texture.

## See Also

### Specifying Texture Origin Options

static let bottomLeft: MTKTextureLoader.Origin

An option for specifying images that should be flipped only to put their origin in the bottom-left corner.

static let flippedVertically: MTKTextureLoader.Origin

An option that specifies that images should always be flipped.

