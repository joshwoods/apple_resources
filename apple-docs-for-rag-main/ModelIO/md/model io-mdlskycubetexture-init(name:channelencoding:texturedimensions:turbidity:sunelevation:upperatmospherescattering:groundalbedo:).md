

- Model I/O
- MDLSkyCubeTexture
-  init(name:channelEncoding:textureDimensions:turbidity:sunElevation:upperAtmosphereScattering:groundAlbedo:) 

Initializer

# init(name:channelEncoding:textureDimensions:turbidity:sunElevation:upperAtmosphereScattering:groundAlbedo:)

Initializes a sky cube texture object with the specified parameters.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    name: String?,
    channelEncoding: MDLTextureChannelEncoding,
    textureDimensions: vector_int2,
    turbidity: Float,
    sunElevation: Float,
    upperAtmosphereScattering: Float,
    groundAlbedo: Float
)
```

## Parameters 

`name`  

The name property for the new texture object.

`channelEncoding`  

The data format for each channel value per texel—for example, 8-bit integer or 32-bit floating point. For possible values, see MDLTextureChannelEncoding.

`textureDimensions`  

The texel dimensions (width and height) of the texture image.

`turbidity`  

The cloudiness or haziness of the simulated sky. See the turbidity property.

`sunElevation`  

The sun’s position in the simulated sky. See the sunElevation property.

`upperAtmosphereScattering`  

A factor that influences the color of the simulated sky. See the upperAtmosphereScattering property.

`groundAlbedo`  

A factor that influences the clarity of the simulated sky. See the groundAlbedo property.

## Return Value

A new sky cube texture object.

## Discussion

The newly created texture is a cube texture; that is, its isCube property is true, and its dimensions property reflects the vertical layout of cube faces.

This initializer does not generate texel data; the MDLSkyCubeTexture class automatically generates data and caches it for reuse when you use one of the MDLTexture methods listed in Accessing Texture Data.

