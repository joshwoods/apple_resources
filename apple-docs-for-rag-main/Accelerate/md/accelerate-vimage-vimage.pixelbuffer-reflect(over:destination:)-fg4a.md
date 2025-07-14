

- Accelerate
- vImage
- vImage.PixelBuffer
-  reflect(over:destination:) 

Instance Method

# reflect(over:destination:)

Reflects an unsigned 16-bit-per-channel, four-channel interleaved pixel buffer over a horizontal or vertical axis.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func reflect(
    over axis: vImage.ReflectionAxis,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.Interleaved16Ux4`.

## Parameters 

`axis`  

The reflection axis.

`destination`  

The destination pixel buffer.

## See Also

### Related Documentation

Applying geometric transforms to images

Reflect, shear, rotate, and scale image buffers using vImage.

### Reflecting images

func reflect(over: vImage.ReflectionAxis, destination: vImage.PixelBuffer&lt;Format>)

Reflects an 8-bit planar pixel buffer over a horizontal or vertical axis.

func reflect(over: vImage.ReflectionAxis, destination: vImage.PixelBuffer&lt;Format>)

Reflects a floating-point 16-bit planar pixel buffer over a horizontal or vertical axis.

func reflect(over: vImage.ReflectionAxis, destination: vImage.PixelBuffer&lt;Format>)

Reflects a 32-bit planar pixel buffer over a horizontal or vertical axis.

func reflect(over: vImage.ReflectionAxis, destination: vImage.PixelBuffer&lt;Format>)

Reflects a floating-point 16-bit-per-channel, two-channel interleaved pixel buffer over a horizontal or vertical axis.

func reflect(over: vImage.ReflectionAxis, destination: vImage.PixelBuffer&lt;Format>)

Reflects an 8-bit-per-channel, four-channel interleaved pixel buffer over a horizontal or vertical axis.

func reflect(over: vImage.ReflectionAxis, destination: vImage.PixelBuffer&lt;Format>)

Reflects a floating-point 16-bit-per-channel, four-channel interleaved pixel buffer over a horizontal or vertical axis.

func reflect(over: vImage.ReflectionAxis, destination: vImage.PixelBuffer&lt;Format>)

Reflects a 32-bit-per-channel, four-channel interleaved pixel buffer over a horizontal or vertical axis.

enum ReflectionAxis

The axis to reflect an image.

