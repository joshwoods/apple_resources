

- Core Graphics
- CGColorRenderingIntent
-  CGColorRenderingIntent.relativeColorimetric 

Case

# CGColorRenderingIntent.relativeColorimetric

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case relativeColorimetric
```

## Discussion

Map colors outside of the gamut of the output device to the closest possible match inside the gamut of the output device. This can produce a clipping effect, where two different color values in the gamut of the graphics context are mapped to the same color value in the output device’s gamut. The relative colorimetric shifts all colors (including those within the gamut) to account for the difference between the white point of the graphics context and the white point of the output device.

## See Also

### Constants

case defaultIntent

The default rendering intent for the graphics context.

case absoluteColorimetric

case perceptual

Preserve the visual relationship between colors by compressing the gamut of the graphics context to fit inside the gamut of the output device. Perceptual intent is good for photographs and other complex, detailed images.

case saturation

