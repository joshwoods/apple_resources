

- RealityKit
- TextureResource
- TextureResource.Format
-  raw(pixelFormat:) 

Type Method

# raw(pixelFormat:)

Indicates a texture for unmodified use by a shader.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
static func raw(pixelFormat: MTLPixelFormat) -> TextureResource.Format
```

## Discussion

The created texture uses the TextureResource.Semantic.raw semantic.

## See Also

### Creating the format

static func color(TextureResource.Format.ColorSpace, pixelFormat: MTLPixelFormat) -> TextureResource.Format

Indicates that a texture contains color data to interpret in a specific color space.

static func normal(TextureResource.Format.NormalEncoding, pixelFormat: MTLPixelFormat) -> TextureResource.Format

Indicates that a texture is a normal map.

