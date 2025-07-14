

- Accelerate
- vImage
- vImage.PixelBuffer
-  boxConvolve(kernelSize:edgeMode:destination:) 

Instance Method

# boxConvolve(kernelSize:edgeMode:destination:)

Convolves a multiple-plane 8-bit-per-channel pixel buffer with a box filter.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func boxConvolve(
    kernelSize: vImage.Size,
    edgeMode: vImage.EdgeMode,
    destination: vImage.PixelBuffer
)
```

Available when `Format` conforms to `MultiplePlanePixelFormat` and `Format.ComponentType` is `UInt8`.

## Parameters 

`kernelSize`  

The convolution kernel size. The operation interprets even dimensions as the next odd number.

`edgeMode`  

The convolution edge mode.

`destination`  

The destination pixel buffer.

## See Also

### Related Documentation

Blurring an image

Filter an image by convolving it with custom and high-speed kernels.

### Box convolution

func boxConvolve(kernelSize: vImage.Size, edgeMode: vImage.EdgeMode&lt;Pixel_8>, destination: vImage.PixelBuffer&lt;Format>)

Convolves an 8-bit planar pixel buffer with a box filter.

func boxConvolve(kernelSize: vImage.Size, edgeMode: vImage.EdgeMode&lt;Pixel_8888>, destination: vImage.PixelBuffer&lt;Format>)

Convolves an 8-bit-per-channel, 4-channel interleaved pixel buffer with a box filter.

func boxConvolved(kernelSize: vImage.Size, edgeMode: vImage.EdgeMode&lt;Pixel_8888>) -> vImage.PixelBuffer&lt;Format>

Returns a box-filter convolved 8-bit-per-channel, 4-channel interleaved pixel buffer.

