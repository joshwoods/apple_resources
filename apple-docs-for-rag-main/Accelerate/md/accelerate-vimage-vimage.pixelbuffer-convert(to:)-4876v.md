

- Accelerate
- vImage
- vImage.PixelBuffer
-  convert(to:) 

Instance Method

# convert(to:)

Converts the contents of the floating-point 16-bit planar pixel buffer to 32-bit planar format.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func convert(to destination: vImage.PixelBuffer)
```

Available when `Format` is `vImage.Planar16F`.

## Parameters 

`destination`  

The destination pixel buffer.

## See Also

### Conversion from 16-bit to 32-bit

func convert(to: vImage.PixelBuffer&lt;vImage.InterleavedFx2>)

Converts the contents of the floating-point 16-bit-per-channel, 2-channel interleaved pixel buffer to 32-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Converts the contents of the unsigned 16-bit-per-channel, 4-channel interleaved pixel buffer to 32-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Converts the contents of the floating-point 16-bit-per-channel, 4-channel interleaved pixel buffer to 32-bit-per-channel format.

