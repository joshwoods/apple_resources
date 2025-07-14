

- RealityKit
- TextureResource
-  pixelFormat 

Instance Property

# pixelFormat

The texture’s pixel format.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
var pixelFormat: MTLPixelFormat { get }
```

## See Also

### Describing the texture

var textureType: MTLTextureType

The dimension and arrangement of the texture image data.

var height: Int

The height of the texture image, in pixels.

var width: Int

The width of the texture image, in pixels.

var depth: Int

The depth of the texture image, in pixels.

var arrayLength: Int

The number of slices in the texture array.

var mipmapLevelCount: Int

The number of mipmaps for the texture.

var semantic: TextureResource.Semantic?

The intended usage of the texture resource.

