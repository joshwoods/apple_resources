

- Accelerate
- vImageCVImageFormat
- vImageCVImageFormat.Format
-  vImageCVImageFormat.Format.formatDisparityFloat16 

Case

# vImageCVImageFormat.Format.formatDisparityFloat16

A 16-bit disparity pixel format that describes the normalized shift when comparing two images.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
case formatDisparityFloat16
```

## Discussion

Units are `1 / meters`, that is, `(pixelShift / (pixelFocalLength * baselineInMeters))`.

## See Also

### Disparity format constants

case formatDisparityFloat32

A 32-bit disparity pixel format that describes the normalized shift when comparing two images.

