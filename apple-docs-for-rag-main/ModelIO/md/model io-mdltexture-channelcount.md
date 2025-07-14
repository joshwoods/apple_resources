

- Model I/O
- MDLTexture
-  channelCount 

Instance Property

# channelCount

The number of channels per texel.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var channelCount: Int { get }
```

## Discussion

For example, a grayscale texture has one channel (brightness) per texel, and a color texture may have three (RGB) or four (RGBA) channels per texel.

## See Also

### Examining Texture Attributes

var dimensions: vector_int2

The width and height, in texels, of the texture image.

var rowStride: Int

The number of bytes between the first texel in a row of image data and the first texel in the next row.

var channelEncoding: MDLTextureChannelEncoding

The data format for each channel value per texel.

var isCube: Bool

A Boolean value that indicates whether the texture is a cube textures.

var mipLevelCount: Int

The number of mipmap levels contained in the texture image data.

