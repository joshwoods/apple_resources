

- RealityKit
- TextureResource
-  textureType 

Instance Property

# textureType

The dimension and arrangement of the texture image data.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
var textureType: MTLTextureType { get }
```

## See Also

### Describing the texture

var pixelFormat: MTLPixelFormat

The texture’s pixel format.

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

