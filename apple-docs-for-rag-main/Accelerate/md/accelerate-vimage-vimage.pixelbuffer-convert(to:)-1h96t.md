

- Accelerate
- vImage
- vImage.PixelBuffer
-  convert(to:) 

Instance Method

# convert(to:)

Converts the contents of the floating-point 16-bit-per-channel, 2-channel interleaved pixel buffer to 8-bit-per-channel format.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func convert(to destination: vImage.PixelBuffer)
```

Available when `Format` is `vImage.Interleaved16Fx2`.

## Parameters 

`destination`  

The destination pixel buffer.

## Discussion

This function converts the source values in the range `[0.0, 1.0]` to the destination range `[0, 255]`. The conversion clamps source values to the range `[0.0, 1.0]`.

## See Also

### Conversion from 16-bit to 8-bit

func convert(to: vImage.PixelBuffer&lt;vImage.Planar8>)

Converts the contents of the floating-point 16-bit planar pixel buffer to 8-bit planar format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Converts the contents of the unsigned 16-bit-per-channel, 4-channel interleaved pixel buffer to 8-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Converts the contents of the floating-point 16-bit-per-channel, 4-channel interleaved pixel buffer to 8-bit-per-channel format.

