

- Model I/O
- MDLNoiseTexture
-  init(scalarNoiseWithSmoothness:name:textureDimensions:channelCount:channelEncoding:grayscale:) 

Initializer

# init(scalarNoiseWithSmoothness:name:textureDimensions:channelCount:channelEncoding:grayscale:)

Initializes a noise texture that creates random color noise.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    scalarNoiseWithSmoothness smoothness: Float,
    name: String?,
    textureDimensions: vector_int2,
    channelCount: Int32,
    channelEncoding: MDLTextureChannelEncoding,
    grayscale: Bool
)
```

## Parameters 

`smoothness`  

A value that indicates how similar neighboring texels will be in the resulting texture. The value should be between `0.0` and `1.0`. A value of `1.0` generates a smooth surface.

`name`  

The name property for the new texture object.

`textureDimensions`  

The texel dimensions (width and height) of the texture image.

`channelCount`  

The number of channels per texel—for example, 1 for a grayscale texture, 3 for an RGB color texture, or 4 for RGBA.

`channelEncoding`  

The data format for each channel value per texel—for example, 8-bit integer or 32-bit floating point. For possible values, see MDLTextureChannelEncoding.

`grayscale`  

If true, all four components of each texel will have equal values. If false, all four values are completely randomized.

## Return Value

A new color noise texture object.

## Discussion

A color noise texture has random values for each color channel and can be tiled or mirrored without showing visible borders.

This initializer does not generate texel data; the MDLNoiseTexture class automatically generates data and caches it for reuse when you use one of the MDLTexture methods listed in Accessing Texture Data.

## See Also

### Creating a Noise Texture

init(vectorNoiseWithSmoothness: Float, name: String?, textureDimensions: vector_int2, channelEncoding: MDLTextureChannelEncoding)

Initializes a noise texture that creates random directional noise.

