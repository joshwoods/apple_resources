

- Accelerate
- vImage
-  vImage.Interleaved16Fx4 

Structure

# vImage.Interleaved16Fx4

A four-channel, 16-bit-per-channel, floating-point interleaved buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct Interleaved16Fx4
```

## Topics

### Type Methods

static func makePixel(Pixel_FFFF) -> Pixel_ARGB_16F

Returns a 16-bit floating-point pixel value from a 32-bit floating-point pixel value.

## Relationships

### Conforms To

- InitializableFromCGImage
- PixelFormat
- SinglePlanePixelFormat
- StaticPixelFormat

## See Also

### Type Aliases

typealias StructuringElement

A 2D matrix that represents a morphology kernel.

struct ConvolutionKernel

Constants that describe 1D convolution kernels.

struct ConvolutionKernel2D

A 2D matrix that represents a convolution kernel.

struct DynamicPixelFormat

A buffer that contains pixels with a data type that’s unknown at compile time.

struct Interleaved16Fx2

A two-channel, 16-bit-per-channel, floating-point interleaved buffer.

struct Interleaved16Ux2

A two-channel, 16-bit-per-channel, unsigned-integer interleaved buffer.

struct Interleaved16Ux4

A four-channel, 16-bit-per-channel, unsigned-integer interleaved buffer.

struct Interleaved8x2

A two-channel, 8-bit-per-channel interleaved buffer.

struct Interleaved8x3

A three-channel, 8-bit-per-channel interleaved buffer.

struct Interleaved8x4

A four-channel, 8-bit-per-channel interleaved buffer.

struct InterleavedFx2

A two-channel, 32-bit-per-channel, floating-point interleaved buffer.

struct InterleavedFx3

A three-channel, 32-bit-per-channel, floating-point interleaved buffer.

struct InterleavedFx4

A four-channel, 32-bit-per-channel, floating-point interleaved buffer.

struct MultidimensionalLookupTable

A multidimensional lookup table.

struct Options

Set flags on vImage operations to specify processing options.

