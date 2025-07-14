

- Model I/O
- MDLNormalMapTexture
-  init(byGeneratingNormalMapWith:name:smoothness:contrast:) 

Initializer

# init(byGeneratingNormalMapWith:name:smoothness:contrast:)

Initializes a normal map to be generated from the specified texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    byGeneratingNormalMapWith sourceTexture: MDLTexture,
    name: String?,
    smoothness: Float,
    contrast: Float
)
```

## Parameters 

`sourceTexture`  

The texture from which to generate a normal map.

`name`  

The name property for the new texture object.

`smoothness`  

A number between `0.0` and `1.0` indicating how much the texture should be smoothed before the normal map is generated. A value of `0.0` means that the texture is not smoothed at all before being processed.

`contrast`  

A value used to magnify the effect of the generated normal map. A value of `1.0` indicates no magnification is applied.

## Return Value

A new normal map texture object.

## Discussion

This initializer does not generate texel data; the MDLNormalMapTexture class automatically generates data when you use one of the MDLTexture methods listed in Accessing Texture Data. The generated texture uses the same dimensions and other properties as the source texture.

