

- UIKit
- UIColor
-  init(hue:saturation:brightness:alpha:) 

Initializer

# init(hue:saturation:brightness:alpha:)

Creates a color object using the specified opacity and HSB color space component values.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(
    hue: CGFloat,
    saturation: CGFloat,
    brightness: CGFloat,
    alpha: CGFloat
)
```

## Parameters 

`hue`  

The hue value of the color object. On applications linked for iOS 10 or later, the color is specified in an extended color space, and the input value is never clamped. On earlier versions of iOS, hue values below 0.0 are interpreted as 0.0, and values above 1.0 are interpreted as 1.0.

`saturation`  

The saturation value of the color object. On applications linked for iOS 10 or later, the color is specified in an extended color space, and the input value is never clamped. On earlier versions of iOS, saturation values below 0.0 are interpreted as 0.0, and values above 1.0 are interpreted as 1.0.

`brightness`  

The brightness value of the color object. On applications linked for iOS 10 or later, the color is specified in an extended color space, and the input value is never clamped. On earlier versions of iOS, brightness values below 0.0 are interpreted as 0.0, and values above 1.0 are interpreted as 1.0.

`alpha`  

The opacity value of the color object, specified as a value from 0.0 to 1.0. Alpha values below 0.0 are interpreted as 0.0, and values above 1.0 are interpreted as 1.0.

## Return Value

The color object. The color information represented by this object is in an RGB colorspace. On applications linked for iOS 10 or later, the color is specified in an extended range sRGB color space. On earlier versions of iOS, the color is specified in a device RGB colorspace.

## See Also

### Creating a color from component values

init(white: CGFloat, alpha: CGFloat)

Creates a color object using the specified opacity and grayscale values.

init(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object using the specified opacity and RGB component values.

init(displayP3Red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object using the specified opacity and RGB component values in the Display P3 color space.

init?(named: String)

Creates a color object using the information from the named asset.

init?(named: String, inBundle: Bundle?, compatibleWithTraitCollection: UITraitCollection?)

Creates a color object using the named asset that’s compatible with the specified trait collection.

