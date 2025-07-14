

- AppKit
- NSColor
-  init(calibratedHue:saturation:brightness:alpha:) 

Initializer

# init(calibratedHue:saturation:brightness:alpha:)

Creates a color object using the given opacity and HSB color space components.

macOS

``` source
init(
    calibratedHue hue: CGFloat,
    saturation: CGFloat,
    brightness: CGFloat,
    alpha: CGFloat
)
```

## Parameters 

`hue`  

The hue component of the color object in the HSB color space.

`saturation`  

The saturation component of the color object in the HSB color space.

`brightness`  

The brightness (or value) component of the color object in the HSB color space.

`alpha`  

The opacity value of the color object,

## Return Value

The color object.

## Discussion

Values below 0.0 are interpreted as 0.0, and values above 1.0 are interpreted as 1.0.

## See Also

### Related Documentation

func getHue(UnsafeMutablePointer&lt;CGFloat>?, saturation: UnsafeMutablePointer&lt;CGFloat>?, brightness: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s HSB component and opacity values in the respective arguments.

init(calibratedRed: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity and RGB components.

### Creating a Color Using HSB Components

init(deviceHue: CGFloat, saturation: CGFloat, brightness: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity value and HSB color space components.

init(hue: CGFloat, saturation: CGFloat, brightness: CGFloat, alpha: CGFloat)

Creates a color object with the specified hue, saturation, brightness, and alpha channel values.

init(colorSpace: NSColorSpace, hue: CGFloat, saturation: CGFloat, brightness: CGFloat, alpha: CGFloat)

Creates a color object with the specified color space, hue, saturation, brightness, and alpha channel values.

