

- Accelerate
- vImage
- vImage.PixelBuffer
-  scale(useFloat16Accumulator:destination:) 

Instance Method

# scale(useFloat16Accumulator:destination:)

Scales a floating-point 16-bit planar pixel buffer to fit the destination buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func scale(
    useFloat16Accumulator: Bool = false,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.Planar16F`.

## Parameters 

`useFloat16Accumulator`  

A Boolean value that specifies that the function uses faster, but lower-precision, internal arithmetic. For more information, see kvImageUseFP16Accumulator.

`destination`  

The destination pixel buffer.

## See Also

### Related Documentation

Applying geometric transforms to images

Reflect, shear, rotate, and scale image buffers using vImage.

### Scaling images

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales an 8-bit planar pixel buffer to fit the destination buffer.

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales an unsigned 16-bit planar pixel buffer to fit the destination buffer.

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales a 32-bit planar pixel buffer to fit the destination buffer.

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales an 8-bit-per-channel, two-channel interleaved pixel buffer to fit the destination buffer.

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales an unsigned 16-bit-per-channel, two-channel interleaved pixel buffer to fit the destination buffer.

func scale(useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Scales a floating-point 16-bit-per-channel, two-channel interleaved pixel buffer to fit the destination buffer.

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales an 8-bit-per-channel, four-channel interleaved pixel buffer to fit the destination buffer.

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales an unsigned 16-bit-per-channel, four-channel interleaved pixel buffer to fit the destination buffer.

func scale(useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Scales a floating-point 16-bit-per-channel, four-channel interleaved pixel buffer to fit the destination buffer.

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales a 32-bit-per-channel, four-channel interleaved pixel buffer to fit the destination buffer.

