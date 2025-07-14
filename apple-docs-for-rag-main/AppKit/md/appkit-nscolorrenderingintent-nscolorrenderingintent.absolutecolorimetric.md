

- AppKit
- NSColorRenderingIntent
-  NSColorRenderingIntent.absoluteColorimetric 

Case

# NSColorRenderingIntent.absoluteColorimetric

Map colors outside of the gamut of the output device to the closest possible match inside the gamut of the output device.

macOS 10.5+

``` source
case absoluteColorimetric
```

## Discussion

This operation can produce a clipping effect, where two different color values in the gamut of the graphics context are mapped to the same color value in the output device’s gamut. Unlike the relative colorimetric, absolute colorimetric does not modify colors inside the gamut of the output device.

## See Also

### Constants

case `default`

Use the default rendering intent for the graphics context.

case relativeColorimetric

Map colors outside of the gamut of the output device to the closest possible match inside the gamut of the output device.

case perceptual

Preserve the visual relationship between colors by compressing the gamut of the graphics context to fit inside the gamut of the output device.

case saturation

Preserve the relative saturation value of the colors when converting into the gamut of the output device.

