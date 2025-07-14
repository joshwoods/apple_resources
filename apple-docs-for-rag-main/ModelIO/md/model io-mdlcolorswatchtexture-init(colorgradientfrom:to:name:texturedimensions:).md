

- Model I/O
- MDLColorSwatchTexture
-  init(colorGradientFrom:to:name:textureDimensions:) 

Initializer

# init(colorGradientFrom:to:name:textureDimensions:)

Initializes a texture that creates a vertical gradient between two colors.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    colorGradientFrom color1: CGColor,
    to color2: CGColor,
    name: String?,
    textureDimensions: vector_int2
)
```

## Parameters 

`color1`  

The color at the top of the gradient.

`color2`  

The color at the bottom of the gradient.

`name`  

The name property for the new texture object.

`textureDimensions`  

The texel dimensions (width and height) of the texture image.

## Return Value

A new color swatch texture object.

## Discussion

Model I/O interpolates between the `color1` and `color2` colors by hue, saturation, and lightness to create a color gradient when generating texture data.

This initializer does not generate texel data; the MDLColorSwatchTexture class automatically generates data and caches it for reuse when you use one of the MDLTexture methods listed in Accessing Texture Data.

## See Also

### Creating a Color Swatch Texture

init(colorTemperatureGradientFrom: Float, toColorTemperature: Float, name: String?, textureDimensions: vector_int2)

Initializes a texture that creates a vertical gradient between two color temperatures.

