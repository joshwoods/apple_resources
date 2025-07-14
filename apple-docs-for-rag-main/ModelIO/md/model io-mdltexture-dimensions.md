

- Model I/O
- MDLTexture
-  dimensions 

Instance Property

# dimensions

The width and height, in texels, of the texture image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var dimensions: vector_int2 { get }
```

## Discussion

If the texture contains multiple mipmap levels (the mipLevelCount value is greater than zero), this property reflects the base (largest) mipmap level.

If the texture is a cube texture (the isCube value is true), this property reflects the vertical arrangement of cube faces in the texture image data. That is, the texture’s height is six times its width, and the data represents six square images for the six sides of the cube.

## See Also

### Examining Texture Attributes

var rowStride: Int

The number of bytes between the first texel in a row of image data and the first texel in the next row.

var channelCount: Int

The number of channels per texel.

var channelEncoding: MDLTextureChannelEncoding

The data format for each channel value per texel.

var isCube: Bool

A Boolean value that indicates whether the texture is a cube textures.

var mipLevelCount: Int

The number of mipmap levels contained in the texture image data.

