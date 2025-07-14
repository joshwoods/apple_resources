

- Model I/O
- MDLColorSwatchTexture
-  init(colorTemperatureGradientFrom:toColorTemperature:name:textureDimensions:) 

Initializer

# init(colorTemperatureGradientFrom:toColorTemperature:name:textureDimensions:)

Initializes a texture that creates a vertical gradient between two color temperatures.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    colorTemperatureGradientFrom colorTemperature1: Float,
    toColorTemperature colorTemperature2: Float,
    name: String?,
    textureDimensions: vector_int2
)
```

## Parameters 

`colorTemperature1`  

The black-body color temperature, in Kelvins, at the top of the gradient.

`colorTemperature2`  

The black-body color temperature, in Kelvins, at the bottom of the gradient.

`name`  

The name property for the new texture object.

`textureDimensions`  

The texel dimensions (width and height) of the texture image.

## Return Value

A new color swatch texture object.

## Discussion

Real-world light sources often measure color of illumination based on a black-body temperature scale. For example, the colors and characterizations of typical home and office light fixtures correspond to the following temperatures:

| Label           | Color                           | Temperature |
|-----------------|---------------------------------|-------------|
| “Soft white”    | Warm, yellowish white           | 2700 K      |
| “Bright white”  | Pale yellowish white            | 3000 K      |
| “Daylight”      | Bright, slightly greenish white | 5000 K      |
| “Cool daylight” | Bright, slightly bluish white   | 6500 K      |

This initializer does not generate texel data; the MDLColorSwatchTexture class automatically generates data and caches it for reuse when you use one of the MDLTexture methods listed in Accessing Texture Data.

## See Also

### Creating a Color Swatch Texture

init(colorGradientFrom: CGColor, to: CGColor, name: String?, textureDimensions: vector_int2)

Initializes a texture that creates a vertical gradient between two colors.

