

- RealityKit
- TextureResource
-  mipmapLevelCount 

Instance Property

# mipmapLevelCount

The number of mipmaps for the texture.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
var mipmapLevelCount: Int { get }
```

## Discussion

Mipmaps are additional copies of the same texture at different resolutions. This property contains the number of different versions of the texture, including the original-size version.

## See Also

### Describing the texture

var textureType: MTLTextureType

The dimension and arrangement of the texture image data.

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

var semantic: TextureResource.Semantic?

The intended usage of the texture resource.

