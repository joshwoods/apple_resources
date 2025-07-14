

- Model I/O
- MDLTexture
-  init(data:topLeftOrigin:name:dimensions:rowStride:channelCount:channelEncoding:isCube:) 

Initializer

# init(data:topLeftOrigin:name:dimensions:rowStride:channelCount:channelEncoding:isCube:)

Initializes a texture object with the specified image data and properties.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    data pixelData: Data?,
    topLeftOrigin: Bool,
    name: String?,
    dimensions: vector_int2,
    rowStride: Int,
    channelCount: Int,
    channelEncoding: MDLTextureChannelEncoding,
    isCube: Bool
)
```

## Parameters 

`pixelData`  

The texture image data. Pass `nil` for subclasses of MDLTexture that create their own texture data.

`topLeftOrigin`  

If true, the image data is organized such that its first pixel represents the top left corner of the image. If false, the first pixel represents the bottom left corner of the image.

`name`  

A descriptive name for the texture. Use the name property to reference this name after initialization.

`dimensions`  

The texel dimensions (width and height) of the texture image.

`rowStride`  

The number of bytes between the first texel in a row of image data and the first texel in the next row. If zero, the texture does not support direct addressing of texels—this is the case for some compressed texture formats.

`channelCount`  

The number of channels per texel—for example, 1 for a grayscale texture, 3 for an RGB color texture, or 4 for RGBA.

`channelEncoding`  

The data format for each channel value per texel—for example, 8-bit integer or 32-bit floating point. For possible values, see MDLTextureChannelEncoding.

`isCube`  

If true, the image data represents an arrangement of six square images, each of which is a face for a cube texture. If false, the texture is a single 2D image.

## Return Value

A new texture object.

