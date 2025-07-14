

- Accelerate
- vImage
- vImage.PixelBuffer
-  Pixel formats 

API Collection

# Pixel formats

Specify a pixel buffer’s bit depth, number of channels, and data storage format.

## Topics

### Planar pixel formats

struct Planar8

A single-channel, 8-bit-per-channel, unsigned-integer buffer.

struct Planar16U

A single-channel, 16-bit-per-channel, unsigned-integer buffer.

struct Planar16F

A single-channel, 16-bit-per-channel, floating-point buffer.

struct PlanarF

A single-channel, 32-bit-per-channel, floating-point buffer.

### Multiple-plane pixel formats

struct Planar8x2

A pixel buffer that contains two homogeneous 8-bit planes, for example, CbCr.

struct Planar8x3

A pixel buffer that contains three homogeneous 8-bit planes, for example, RGB.

struct Planar8x4

A pixel buffer that contains four homogeneous 8-bit planes, for example, RGBA or CMYK.

struct PlanarFx2

A pixel buffer that contains two homogeneous 32-bit, floating-point planes, for example, CbCr.

struct PlanarFx3

A pixel buffer that contains three homogeneous 32-bit, floating-point planes, for example, RGB.

struct PlanarFx4

A pixel buffer that contains four homogeneous 32-bit, floating-point planes, for example, RGBA or CMYK.

### Interleaved pixel formats

struct Interleaved8x2

A two-channel, 8-bit-per-channel interleaved buffer.

struct Interleaved8x3

A three-channel, 8-bit-per-channel interleaved buffer.

struct Interleaved8x4

A four-channel, 8-bit-per-channel interleaved buffer.

struct Interleaved16Ux2

A two-channel, 16-bit-per-channel, unsigned-integer interleaved buffer.

struct Interleaved16Ux4

A four-channel, 16-bit-per-channel, unsigned-integer interleaved buffer.

struct Interleaved16Fx2

A two-channel, 16-bit-per-channel, floating-point interleaved buffer.

struct Interleaved16Fx4

A four-channel, 16-bit-per-channel, floating-point interleaved buffer.

struct InterleavedFx2

A two-channel, 32-bit-per-channel, floating-point interleaved buffer.

struct InterleavedFx3

A three-channel, 32-bit-per-channel, floating-point interleaved buffer.

struct InterleavedFx4

A four-channel, 32-bit-per-channel, floating-point interleaved buffer.

### Dynamic pixel formats

struct DynamicPixelFormat

A buffer that contains pixels with a data type that’s unknown at compile time.

### Protocols

protocol PixelFormat

A pixel buffer pixel format.

protocol StaticPixelFormat

A pixel format that’s known at compile time.

protocol InitializableFromCGImage

A pixel format that supports initialization from a Core Graphics image.

protocol SinglePlanePixelFormat

A pixel format that contains a single underlying vImage buffer.

protocol MultiplePlanePixelFormat

A pixel format that contains multiple homogeneous planes represented by multiple underlying vImage buffers.

## See Also

### Pixel buffer essentials

Creating vImage pixel buffers

Allocate and initialize pixel buffers from raw pixel data, Core Graphics images, and Core Video buffers.

Working with underlying data

Access a pixel buffer’s underlying pixel data.

