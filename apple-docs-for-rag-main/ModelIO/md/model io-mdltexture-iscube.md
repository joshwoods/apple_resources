

- Model I/O
- MDLTexture
-  isCube 

Instance Property

# isCube

A Boolean value that indicates whether the texture is a cube textures.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var isCube: Bool { get set }
```

## Discussion

Cube textures are used in skybox rendering, light probes, and environment maps. If this property’s value is true, the texture object represents a cube texture. In this case, the texture’s image data (accessible with the methods in Accessing Texture Data) contains six square images arranged vertically. The images represent the +X, -X, +Y, -Y, +Z, and -Z faces of the cube (in that order), and the dimensions property reflects this arrangement (height is six times width).

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

var mipLevelCount: Int

The number of mipmap levels contained in the texture image data.

