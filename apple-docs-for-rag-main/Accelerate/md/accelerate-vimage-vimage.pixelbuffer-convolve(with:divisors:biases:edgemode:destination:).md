

- Accelerate
- vImage
- vImage.PixelBuffer
-  convolve(with:divisors:biases:edgeMode:destination:) 

Instance Method

# convolve(with:divisors:biases:edgeMode:destination:)

Convolves an 8-bit-per-channel, 4-channel interleaved pixel buffer with separate kernels for each channel.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func convolve(
    with kernels: (vImage.ConvolutionKernel2D, vImage.ConvolutionKernel2D, vImage.ConvolutionKernel2D, vImage.ConvolutionKernel2D),
    divisors: (Int32, Int32, Int32, Int32)?,
    biases: (Int32, Int32, Int32, Int32) = (0, 0, 0, 0),
    edgeMode: vImage.EdgeMode,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.Interleaved8x4`.

## Parameters 

`kernels`  

The convolution kernels.

`divisors`  

An optional tuple of four values that the operation adds to the sum of weighted pixels before it applies the divisor.

`biases`  

A tuple of four values that the operation adds to the sum of weighted pixels before it applies the divisor.

`edgeMode`  

The convolution edge mode.

`destination`  

The destination pixel buffer.

## See Also

### Related Documentation

Blurring an image

Filter an image by convolving it with custom and high-speed kernels.

### General convolution

func convolve(with: vImage.ConvolutionKernel2D&lt;Int16>, divisor: Int32?, bias: Int32?, edgeMode: vImage.EdgeMode&lt;Pixel_8>, destination: vImage.PixelBuffer&lt;Format>)

Convolves an 8-bit planar pixel buffer.

func convolve(with: vImage.ConvolutionKernel2D&lt;Float>, bias: Float?, edgeMode: vImage.EdgeMode&lt;Pixel_16F>, useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Convolves a floating-point 16-bit planar pixel buffer.

func convolve(with: vImage.ConvolutionKernel2D&lt;Float>, bias: Float?, edgeMode: vImage.EdgeMode&lt;Pixel_F>, destination: vImage.PixelBuffer&lt;Format>)

Convolves a 32-bit planar pixel buffer.

func convolve(with: vImage.ConvolutionKernel2D&lt;Int16>, divisor: Int32?, bias: Int32?, edgeMode: vImage.EdgeMode&lt;Pixel_8888>, destination: vImage.PixelBuffer&lt;Format>)

Convolves an 8-bit-per-channel, 4-channel interleaved pixel buffer.

func convolve(with: vImage.ConvolutionKernel2D&lt;Float>, bias: Float?, edgeMode: vImage.EdgeMode&lt;Pixel_ARGB_16F>, useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Convolves a floating-point 16-bit-per-channel, 4-channel interleaved pixel buffer.

func convolve(with: vImage.ConvolutionKernel2D&lt;Float>, bias: Float?, edgeMode: vImage.EdgeMode&lt;Pixel_FFFF>, destination: vImage.PixelBuffer&lt;Format>)

Convolves a 32-bit-per-channel, 4-channel interleaved pixel buffer.

func convolve(with: vImage.ConvolutionKernel2D&lt;Int16>, divisor: Int32?, bias: Int32?, edgeMode: vImage.EdgeMode&lt;Pixel_8>, destination: vImage.PixelBuffer&lt;Format>)

Convolves an 8-bit multiple plane pixel buffer.

func convolve(with: vImage.ConvolutionKernel2D&lt;Float>, bias: Float?, edgeMode: vImage.EdgeMode&lt;Pixel_F>, destination: vImage.PixelBuffer&lt;Format>)

Convolves a 32-bit multiple plane pixel buffer.

enum EdgeMode

Constants that specify edge modes for convolution operations.

struct ConvolutionKernel2D

A 2D matrix that represents a convolution kernel.

