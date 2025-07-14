

- AppKit
- NSColor
-  init(genericGamma22White:alpha:) 

Initializer

# init(genericGamma22White:alpha:)

Returns a color object with the specified white and alpha values in the GenericGamma22 colorspace.

macOS 10.7+

``` source
init(
    genericGamma22White white: CGFloat,
    alpha: CGFloat
)
```

## Parameters 

`white`  

The white value of the color object.

`alpha`  

The opacity value of the color object.

## Return Value

The color object.

## Discussion

Values below 0.0 are interpreted as 0.0, and values above 1.0 are interpreted as 1.0.

## See Also

### Related Documentation

init(srgbRed: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object from the specified components in the sRGB colorspace.

init(deviceHue: CGFloat, saturation: CGFloat, brightness: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity value and HSB color space components.

init(calibratedRed: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity and RGB components.

### Creating a Color Using White Components

init(white: CGFloat, alpha: CGFloat)

Creates a color object with the specified brightness and alpha channel values.

init(calibratedWhite: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity and grayscale values.

init(deviceWhite: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity and grayscale values.

