

- SwiftUI
- GraphicsContext
- GraphicsContext.Shading
-  color(\_:white:opacity:) 

Type Method

# color(\_:white:opacity:)

Returns a shading instance that fills with a monochrome color in the given color space.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func color(
    _ colorSpace: Color.RGBColorSpace = .sRGB,
    white: Double,
    opacity: Double = 1
) -> GraphicsContext.Shading
```

## Parameters 

`colorSpace`  

The RGB color space used to define the color. The default is Color.RGBColorSpace.sRGB.

`white`  

The value to use for each of the red, green, and blue components of the color.

`opacity`  

The opacity of the color. The default is `1`, which means fully opaque.

## Return Value

A shading instance filled with a color.

## See Also

### Colors

static func color(Color) -> GraphicsContext.Shading

Returns a shading instance that fills with a color.

static func color(Color.RGBColorSpace, red: Double, green: Double, blue: Double, opacity: Double) -> GraphicsContext.Shading

Returns a shading instance that fills with a color in the given color space.

