

- Model I/O
- MDLTexture
-  rowStride 

Instance Property

# rowStride

The number of bytes between the first texel in a row of image data and the first texel in the next row.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var rowStride: Int { get }
```

## Discussion

If this value is zero, the texture does not support direct addressing of texels—this is the case for some compressed texture formats.

## See Also

### Examining Texture Attributes

var dimensions: vector_int2

The width and height, in texels, of the texture image.

var channelCount: Int

The number of channels per texel.

var channelEncoding: MDLTextureChannelEncoding

The data format for each channel value per texel.

var isCube: Bool

A Boolean value that indicates whether the texture is a cube textures.

var mipLevelCount: Int

The number of mipmap levels contained in the texture image data.

