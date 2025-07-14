

- Core Graphics
- CGColorRenderingIntent
-  CGColorRenderingIntent.saturation 

Case

# CGColorRenderingIntent.saturation

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case saturation
```

## Discussion

Preserve the relative saturation value of the colors when converting into the gamut of the output device. The result is an image with bright, saturated colors. Saturation intent is good for reproducing images with low detail, such as presentation charts and graphs.

## See Also

### Constants

case defaultIntent

The default rendering intent for the graphics context.

case absoluteColorimetric

case relativeColorimetric

case perceptual

Preserve the visual relationship between colors by compressing the gamut of the graphics context to fit inside the gamut of the output device. Perceptual intent is good for photographs and other complex, detailed images.

