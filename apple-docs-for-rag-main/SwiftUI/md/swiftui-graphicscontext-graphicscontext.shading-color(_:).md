

- SwiftUI
- GraphicsContext
- GraphicsContext.Shading
-  color(\_:) 

Type Method

# color(\_:)

Returns a shading instance that fills with a color.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func color(_ color: Color) -> GraphicsContext.Shading
```

## Parameters 

`color`  

A Color instance that defines the color of the shading.

## Return Value

A shading instance filled with a color.

## See Also

### Colors

static func color(Color.RGBColorSpace, red: Double, green: Double, blue: Double, opacity: Double) -> GraphicsContext.Shading

Returns a shading instance that fills with a color in the given color space.

static func color(Color.RGBColorSpace, white: Double, opacity: Double) -> GraphicsContext.Shading

Returns a shading instance that fills with a monochrome color in the given color space.

