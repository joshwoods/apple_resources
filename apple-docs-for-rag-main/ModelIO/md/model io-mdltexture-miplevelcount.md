

- Model I/O
- MDLTexture
-  mipLevelCount 

Instance Property

# mipLevelCount

The number of mipmap levels contained in the texture image data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var mipLevelCount: Int { get }
```

## Discussion

Mipmapping is a technique that uses multiple sizes of a texture image to increase rendering performance. If this property’s value is zero, the texture contains a single image, whose size matches the dimensions property. If this value is 1, the texture contains an additional image at half the original dimensions; if this value is 2, the texture contains images at the original size, at half size, and at quarter size; and so on.

## See Also

### Examining Texture Attributes

var dimensions: vector_int2

The width and height, in texels, of the texture image.

var rowStride: Int

The number of bytes between the first texel in a row of image data and the first texel in the next row.

var channelCount: Int

The number of channels per texel.

var channelEncoding: MDLTextureChannelEncoding

The data format for each channel value per texel.

var isCube: Bool

A Boolean value that indicates whether the texture is a cube textures.

