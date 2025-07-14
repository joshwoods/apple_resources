

- SwiftUI
- Color
-  Color.RGBColorSpace 

Enumeration

# Color.RGBColorSpace

A profile that specifies how to interpret a color value for display.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum RGBColorSpace
```

## Topics

### Getting color spaces

case sRGB

The extended red, green, blue (sRGB) color space.

case sRGBLinear

The extended sRGB color space with a linear transfer function.

case displayP3

The Display P3 color space.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a color from component values

init(hue: Double, saturation: Double, brightness: Double, opacity: Double)

Creates a constant color from hue, saturation, and brightness values.

init(Color.RGBColorSpace, white: Double, opacity: Double)

Creates a constant grayscale color.

init(Color.RGBColorSpace, red: Double, green: Double, blue: Double, opacity: Double)

Creates a constant color from red, green, and blue component values.

