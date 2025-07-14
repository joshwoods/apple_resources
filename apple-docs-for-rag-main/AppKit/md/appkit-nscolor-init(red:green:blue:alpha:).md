

- AppKit
- NSColor
-  init(red:green:blue:alpha:) 

Initializer

# init(red:green:blue:alpha:)

Creates a color object with the specified red, green, blue, and alpha channel values.

macOS 10.9+

``` source
init(
    red: CGFloat,
    green: CGFloat,
    blue: CGFloat,
    alpha: CGFloat
)
```

## Parameters 

`red`  

The red channel value. If the value is outside of the range `0–1.0`, the extended sRGB color space is used.

`green`  

The green channel value. If the value is outside of the range `0–1.0`, the extended sRGB color space is used.

`blue`  

The blue channel value. If the value is outside of the range `0–1.0`, the extended sRGB color space is used.

`alpha`  

The alpha (opacity), specified as a value from `0-1.0`. Alpha values below `0` are interpreted as `0.0`, and values above `1.0` are interpreted as `1.0`.

## Discussion

This method accepts extended color component values. If the red, green, blue, or alpha values are outside of the `0-1.0` range, the method creates a color in the extended range color space. This method is provided for easier reuse of code that uses UIColor in iOS.

Where possible, it is preferable to specify the colorspace explicitly using the init(srgbRed:green:blue:alpha:) or init(genericGamma22White:alpha:) method.

## See Also

### Creating a Color Using RGB Components

init(srgbRed: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object from the specified components in the sRGB colorspace.

init(displayP3Red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object from the specified components in the Display P3 color space.

init(calibratedRed: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity and RGB components.

init(deviceRed: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity value and RGB components.

