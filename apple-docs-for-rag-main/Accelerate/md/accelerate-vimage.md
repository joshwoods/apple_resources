

- Accelerate
-  vImage 

Enumeration

# vImage

An enumeration that acts as a namespace for Swift overlays to vImage.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
enum vImage
```

## Topics

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

struct Interleaved16Fx4

A four-channel, 16-bit-per-channel, floating-point interleaved buffer.

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

struct PixelBuffer

An image buffer that stores an image’s pixel data, dimensions, bit depth, and number of channels.

struct Planar16F

A single-channel, 16-bit-per-channel, floating-point buffer.

struct Planar16U

A single-channel, 16-bit-per-channel, unsigned-integer buffer.

struct Planar8

A single-channel, 8-bit-per-channel, unsigned-integer buffer.

struct Planar8x2

A pixel buffer that contains two homogeneous 8-bit planes, for example, CbCr.

struct Planar8x3

A pixel buffer that contains three homogeneous 8-bit planes, for example, RGB.

struct Planar8x4

A pixel buffer that contains four homogeneous 8-bit planes, for example, RGBA or CMYK.

struct PlanarF

A single-channel, 32-bit-per-channel, floating-point buffer.

struct PlanarFx2

A pixel buffer that contains two homogeneous 32-bit, floating-point planes, for example, CbCr.

struct PlanarFx3

A pixel buffer that contains three homogeneous 32-bit, floating-point planes, for example, RGB.

struct PlanarFx4

A pixel buffer that contains four homogeneous 32-bit, floating-point planes, for example, RGBA or CMYK.

struct Size

A structure that contains width and height values.

### Enumerations

enum BlendMode

Constants that specify an alpha blending mode.

enum BufferType

Codes that represent vImage buffer types.

enum ChannelOrdering

Constants that specify the channel ordering of a pixel buffer.

enum CompositeMode

Constants that specify whether the format of layers is premultiplied or nonpremultiplied.

enum EdgeMode

Constants that specify edge modes for convolution operations.

enum Error

An error that occurs during a vImage operation.

enum FloodFillConnectivity

enum Gamma

Describes either a used-defined or constant gamma.

enum MorphologyOperation

Describes which morphology operation to perform.

enum ReflectionAxis

The axis to reflect an image.

enum Rotation

The angle to rotate an image.

enum ShearDirection

The shear direction.

