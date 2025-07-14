

- SwiftUI
- Color
- Color.RGBColorSpace
-  Color.RGBColorSpace.sRGBLinear 

Case

# Color.RGBColorSpace.sRGBLinear

The extended sRGB color space with a linear transfer function.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case sRGBLinear
```

## Discussion

This color space has the same colorimetry as Color.RGBColorSpace.sRGB, but uses a linear transfer function.

Standard sRGB color spaces clamp the red, green, and blue components of a color to a range of `0` to `1`, but SwiftUI colors use an extended sRGB color space, so you can use component values outside that range.

## See Also

### Getting color spaces

case sRGB

The extended red, green, blue (sRGB) color space.

case displayP3

The Display P3 color space.

