

- Model I/O
- MDLNoiseTexture
-  init(vectorNoiseWithSmoothness:name:textureDimensions:channelEncoding:) 

Initializer

# init(vectorNoiseWithSmoothness:name:textureDimensions:channelEncoding:)

Initializes a noise texture that creates random directional noise.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    vectorNoiseWithSmoothness smoothness: Float,
    name: String?,
    textureDimensions: vector_int2,
    channelEncoding: MDLTextureChannelEncoding
)
```

## Parameters 

`smoothness`  

A value that indicates how similar neighboring texels will be in the resulting texture. The value should be between `0.0` and `1.0`. A value of `1.0` generates a smooth surface.

`name`  

The name property for the new texture object.

`textureDimensions`  

The texel dimensions (width and height) of the texture image.

`channelEncoding`  

The data format for each channel value per texel—for example, 8-bit integer or 32-bit floating point. For possible values, see MDLTextureChannelEncoding.

## Return Value

A new directional noise texture object.

## Discussion

Unlike a color noise texture, in which the RGBA channels are independently randomized, a directional noise texture treats each texel’s RGB channels together as the XYZ components of a random direction vector, and the A channel as a scalar for the vector’s direction.

This initializer does not generate texel data; the MDLNoiseTexture class automatically generates data and caches it for reuse when you use one of the MDLTexture methods listed in Accessing Texture Data.

## See Also

### Creating a Noise Texture

init(scalarNoiseWithSmoothness: Float, name: String?, textureDimensions: vector_int2, channelCount: Int32, channelEncoding: MDLTextureChannelEncoding, grayscale: Bool)

Initializes a noise texture that creates random color noise.

