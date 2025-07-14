

- AppKit
- NSColor
-  init(calibratedRed:green:blue:alpha:) 

Initializer

# init(calibratedRed:green:blue:alpha:)

Creates a color object using the given opacity and RGB components.

macOS

``` source
init(
    calibratedRed red: CGFloat,
    green: CGFloat,
    blue: CGFloat,
    alpha: CGFloat
)
```

## Parameters 

`red`  

The red component of the color object.

`green`  

The green component of the color object.

`blue`  

The blue component of the color object.

`alpha`  

The opacity value of the color object.

## Return Value

The color object.

## Discussion

Values below 0.0 are interpreted as 0.0, and values above 1.0 are interpreted as 1.0.

## See Also

### Related Documentation

func getRed(UnsafeMutablePointer&lt;CGFloat>?, green: UnsafeMutablePointer&lt;CGFloat>?, blue: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s RGB component and opacity values in the respective arguments.

init(calibratedHue: CGFloat, saturation: CGFloat, brightness: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity and HSB color space components.

### Creating a Color Using RGB Components

init(srgbRed: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object from the specified components in the sRGB colorspace.

init(displayP3Red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object from the specified components in the Display P3 color space.

init(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object with the specified red, green, blue, and alpha channel values.

init(deviceRed: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity value and RGB components.

