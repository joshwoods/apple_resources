

- AppKit
- NSColorRenderingIntent
-  NSColorRenderingIntent.saturation 

Case

# NSColorRenderingIntent.saturation

Preserve the relative saturation value of the colors when converting into the gamut of the output device.

macOS 10.5+

``` source
case saturation
```

## Discussion

The result is an image with bright, saturated colors. Saturation intent is good for reproducing images with low detail, such as presentation charts and graphs.

## See Also

### Constants

case `default`

Use the default rendering intent for the graphics context.

case absoluteColorimetric

Map colors outside of the gamut of the output device to the closest possible match inside the gamut of the output device.

case relativeColorimetric

Map colors outside of the gamut of the output device to the closest possible match inside the gamut of the output device.

case perceptual

Preserve the visual relationship between colors by compressing the gamut of the graphics context to fit inside the gamut of the output device.

