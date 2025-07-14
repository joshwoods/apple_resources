

- Accelerate
- vImage
- vImage.PixelBuffer
-  Creating vImage pixel buffers 

API Collection

# Creating vImage pixel buffers

Allocate and initialize pixel buffers from raw pixel data, Core Graphics images, and Core Video buffers.

## Topics

### Creating a pixel buffer

init(size: vImage.Size, pixelFormat: Format.Type)

Returns a new multiplane pixel buffer with a size that you specify.

init(size: vImage.Size, pixelFormat: Format.Type)

Returns a new pixel buffer with a size that you specify.

init(width: Int, height: Int, pixelFormat: Format.Type)

Returns a new pixel buffer with a width and height that you specify.

struct Size

A structure that contains width and height values.

### Creating a pixel buffer from raw pixel data

init&lt;U>(pixelValues: U, size: vImage.Size, pixelFormat: Format.Type)

Creates a new pixel buffer by copying the supplied collection of pixel values.

init(data: UnsafeMutableRawPointer, width: Int, height: Int, byteCountPerRow: Int, pixelFormat: Format.Type)

Returns a new buffer that references existing data.

init(data: UnsafeMutableRawPointer, width: Int, height: Int, byteCountPerRow: Int?, pixelFormat: Format.Type)

Calculates the correct bytes per row and returns a new buffer that references existing data.

### Creating a pixel buffer from a Core Graphics image

init(cgImage: CGImage, cgImageFormat: inout vImage_CGImageFormat, pixelFormat: Format.Type) throws

Returns a new pixel buffer initialized from a Core Graphics image.

### Creating a pixel buffer from a Core Video buffer

init(copying: CVPixelBuffer, cvImageFormat: vImageCVImageFormat, cgImageFormat: inout vImage_CGImageFormat, pixelFormat: Format.Type) throws

Initializes a pixel buffer by copying the data from a Core Video pixel buffer.

init(referencing: CVPixelBuffer, converter: vImageConverter, destinationPixelFormat: Format.Type)

Returns a new pixel buffer that references the specified Core Video pixel buffer and populated converter.

init(referencing: CVPixelBuffer, planeIndex: Int, overrideSize: vImage.Size?, pixelFormat: Format.Type)

Initializes a pixel buffer by refencing the data from a single plane of a multiplane Core Video pixel buffer.

### Creating a multiple-plane buffer from an interleaved buffer

init(interleavedBuffer: vImage.PixelBuffer&lt;vImage.Interleaved8x3>)

Creates a 3-channel, 8-bit-per-channel multiple-plane buffer from a 3-channel, 8-bit-per-channel interleaved buffer.

init(interleavedBuffer: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Creates a 4-channel, 8-bit-per-channel mutiple-plane buffer from a 4-channel, 8-bit-per-channel interleaved buffer.

init(interleavedBuffer: vImage.PixelBuffer&lt;vImage.InterleavedFx3>)

Creates a 3-channel, 32-bit-per-channel multiple-plane buffer from a 3-channel, 32-bit-per-channel interleaved buffer.

init(interleavedBuffer: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Creates a 4-channel, 32-bit-per-channel multiple-plane buffer from a 4-channel, 32-bit-per-channel interleaved buffer.

### Creating an interleaved buffer from another buffer

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.Planar8>])

Creates a 2-channel, 8-bit-per-channel interleaved buffer from two 8-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.Planar8>])

Creates a 3-channel, 8-bit-per-channel interleaved buffer from three 8-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.Planar8>])

Creates a 4-channel, 8-bit-per-channel interleaved buffer from four 8-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Creates a 4-channel, 8-bit-per-channel interleaved buffer from four 32-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Creates a 2-channel, 32-bit-per-channel interleaved buffer from two 32-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Creates a 3-channel, 32-bit-per-channel interleaved buffer from three 32-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Creates a 4-channel, 32-bit-per-channel interleaved buffer from four 32-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.Planar16U>])

Creates a 4-channel, 16-bit-per-channel interleaved buffer from four 16-bit planar buffers.

init(lumaSource: vImage.PixelBuffer&lt;vImage.Planar8>, chromaSource: vImage.PixelBuffer&lt;vImage.Interleaved8x2>, conversionInfo: vImage_YpCbCrToARGB)

Creates a 4-channel, 8-bit-per-channel interleaved buffer from a planar Yp buffer and a two-channel interleaved CbCr buffer.

init(interleavedBuffer: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Creates a 4-channel, 32-bit-per-channel interleaved buffer from a 4-channel, 8-bit-per-channel interleaved buffer.

### Creating a multiple-plane buffer from planar buffers

init(planarBuffers: [vImage.PixelBuffer&lt;Format.PlanarPixelFormat>], pixelFormat: Format.Type)

Returns an initialized buffer by copying the specified planar buffers.

### Creating a pixel buffer and image format

static func makeDynamicPixelBufferAndCGImageFormat(cgImage: CGImage) throws -> (pixelBuffer: vImage.PixelBuffer&lt;vImage.DynamicPixelFormat>, cgImageFormat: vImage_CGImageFormat)

Returns a new dynamic pixel format pixel buffer and Core Graphics image format structure from a Core Graphics image.

static func makePixelBufferAndCGImageFormat(cgImage: CGImage, pixelFormat: Format.Type) throws -> (pixelBuffer: vImage.PixelBuffer&lt;Format>, cgImageFormat: vImage_CGImageFormat)

Returns a new pixel buffer and Core Graphics image format structure from a Core Graphics image.

## See Also

### Pixel buffer essentials

Pixel formats

Specify a pixel buffer’s bit depth, number of channels, and data storage format.

Working with underlying data

Access a pixel buffer’s underlying pixel data.

