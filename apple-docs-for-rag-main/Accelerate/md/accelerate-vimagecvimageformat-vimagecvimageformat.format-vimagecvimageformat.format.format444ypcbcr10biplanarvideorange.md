

- Accelerate
- vImageCVImageFormat
- vImageCVImageFormat.Format
-  vImageCVImageFormat.Format.format444YpCbCr10BiPlanarVideoRange 

Case

# vImageCVImageFormat.Format.format444YpCbCr10BiPlanarVideoRange

A video-range, two-plane YpCbCr 4:4:4 pixel format with 10 bits per channel.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
case format444YpCbCr10BiPlanarVideoRange
```

## Discussion

This format defines luminance and chrominance data in the range `64...940`, and stores 10 bits in the most significant bits of 16 bits.

## See Also

### 4:4:4 YpCbCr format constants

case format444YpCbCr8

A video-range, component YpCbCr 4:4:4 pixel format with 8 bits per channel and ordered CrYpCb.

case format444YpCbCr10

A component YpCbCr 4:4:4 pixel format with 10 bits per channel.

case format444YpCbCr10BiPlanarFullRange

A full-range, two-plane YpCbCr 4:4:4 pixel format with 10 bits per channel.

