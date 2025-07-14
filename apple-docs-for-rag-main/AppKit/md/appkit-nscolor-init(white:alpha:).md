

- AppKit
- NSColor
-  init(white:alpha:) 

Initializer

# init(white:alpha:)

Creates a color object with the specified brightness and alpha channel values.

macOS 10.9+

``` source
init(
    white: CGFloat,
    alpha: CGFloat
)
```

## Parameters 

`white`  

The brightness. If the value is outside of the range `0–1.0`, the extended sRGB color space is used.

`alpha`  

The alpha (opacity), expressed as a floating-point value in the range `0` (transparent) to `1.0` (opaque). Alpha values below `0` are interpreted as `0.0`, and values above `1.0` are interpreted as `1.0`.

## Discussion

This method accepts extended color component values. If the alpha or white values are outside of the `0-1.0` range, the method creates a color in the extended range or extendedGenericGamma22Gray color space that is compatible with the sRGB colorspace. This method is provided for easier reuse of code that uses UIColor in iOS.

Where possible, it is preferable to specify the colorspace explicitly using the init(srgbRed:green:blue:alpha:) or init(genericGamma22White:alpha:) method.

## See Also

### Creating a Color Using White Components

init(calibratedWhite: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity and grayscale values.

init(deviceWhite: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity and grayscale values.

init(genericGamma22White: CGFloat, alpha: CGFloat)

Returns a color object with the specified white and alpha values in the GenericGamma22 colorspace.

