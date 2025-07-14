

- AppKit
- NSColorRenderingIntent
-  NSColorRenderingIntent.default 

Case

# NSColorRenderingIntent.default

Use the default rendering intent for the graphics context.

macOS 10.5+

``` source
case `default`
```

## See Also

### Constants

case absoluteColorimetric

Map colors outside of the gamut of the output device to the closest possible match inside the gamut of the output device.

case relativeColorimetric

Map colors outside of the gamut of the output device to the closest possible match inside the gamut of the output device.

case perceptual

Preserve the visual relationship between colors by compressing the gamut of the graphics context to fit inside the gamut of the output device.

case saturation

Preserve the relative saturation value of the colors when converting into the gamut of the output device.

