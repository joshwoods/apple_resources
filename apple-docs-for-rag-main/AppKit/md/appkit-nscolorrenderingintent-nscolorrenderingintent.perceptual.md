

- AppKit
- NSColorRenderingIntent
-  NSColorRenderingIntent.perceptual 

Case

# NSColorRenderingIntent.perceptual

Preserve the visual relationship between colors by compressing the gamut of the graphics context to fit inside the gamut of the output device.

macOS 10.5+

``` source
case perceptual
```

## Discussion

Perceptual intent is good for photographs and other complex, detailed images.

## See Also

### Constants

case `default`

Use the default rendering intent for the graphics context.

case absoluteColorimetric

Map colors outside of the gamut of the output device to the closest possible match inside the gamut of the output device.

case relativeColorimetric

Map colors outside of the gamut of the output device to the closest possible match inside the gamut of the output device.

case saturation

Preserve the relative saturation value of the colors when converting into the gamut of the output device.

