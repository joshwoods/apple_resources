

- AppKit
- NSColor
-  init(colorSpace:hue:saturation:brightness:alpha:) 

Initializer

# init(colorSpace:hue:saturation:brightness:alpha:)

Creates a color object with the specified color space, hue, saturation, brightness, and alpha channel values.

macOS 10.12+

``` source
init(
    colorSpace space: NSColorSpace,
    hue: CGFloat,
    saturation: CGFloat,
    brightness: CGFloat,
    alpha: CGFloat
)
```

## Parameters 

`space`  

An `NSColorSpace` object representing a color space. An exception is raised if the color model of the provided color space is not RGB.

`hue`  

The hue (color) component, expressed as a floating-point value in the range 0–1.0.

`saturation`  

The color saturation component, expressed as a floating-point value in the range 0–1.0.

`brightness`  

The brightness component, expressed as a floating-point value in the range 0–1.0.

`alpha`  

The alpha (opacity), expressed as a floating-point value in the range 0 (transparent) to 1.0 (opaque).

## Return Value

The color object.

## See Also

### Creating a Color Using HSB Components

init(calibratedHue: CGFloat, saturation: CGFloat, brightness: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity and HSB color space components.

init(deviceHue: CGFloat, saturation: CGFloat, brightness: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity value and HSB color space components.

init(hue: CGFloat, saturation: CGFloat, brightness: CGFloat, alpha: CGFloat)

Creates a color object with the specified hue, saturation, brightness, and alpha channel values.

