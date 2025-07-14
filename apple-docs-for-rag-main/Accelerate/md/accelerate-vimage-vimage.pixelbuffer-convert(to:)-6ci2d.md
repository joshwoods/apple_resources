

- Accelerate
- vImage
- vImage.PixelBuffer
-  convert(to:) 

Instance Method

# convert(to:)

Converts the contents of the 8-bit-per-channel, 4-channel interleaved pixel buffer to floating-point 16-bit-per-channel format.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func convert(to destination: vImage.PixelBuffer)
```

Available when `Format` is `vImage.Interleaved8x4`.

## Parameters 

`destination`  

The destination pixel buffer.

## Discussion

This function converts the source values in the range `[0, 255]` to the destination range `[0.0, 1.0]`.

## See Also

### Conversion from 8-bit to 16-bit

func convert(to: vImage.PixelBuffer&lt;vImage.Planar16F>)

Converts the contents of the 8-bit planar pixel buffer to floating-point 16-bit planar format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved16Fx2>)

Converts the contents of the 8-bit-per-channel, 2-channel interleaved pixel buffer to floating-point 16-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved16Ux4>)

Converts the contents of the 8-bit-per-channel, 4-channel interleaved pixel buffer to unsigned 16-bit-per-channel format.

