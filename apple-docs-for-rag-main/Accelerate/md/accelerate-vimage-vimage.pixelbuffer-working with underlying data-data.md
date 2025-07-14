

- Accelerate
- vImage
- vImage.PixelBuffer
-  Working with underlying data 

API Collection

# Working with underlying data

Access a pixel buffer’s underlying pixel data.

## Topics

### Converting to an array

func makeArray&lt;U>(of: U.Type, channelCount: Int) -> [U]

Returns an array of `width * height * channelCount` values that’s a copy of the buffer’s visible contents.

### Accessing underlying pixel values

func withUnsafeBufferPointer&lt;R>((UnsafeBufferPointer&lt;Format.ComponentType>) throws -> R) rethrows -> R

Calls the given closure with a pointer to the buffer’s contiguous storage.

func withUnsafeMutableBufferPointer&lt;R>((inout UnsafeMutableBufferPointer&lt;Format.ComponentType>) throws -> R) rethrows -> R

Calls the given closure with a pointer to the buffer’s mutable contiguous storage.

### Accessing underlying vImage buffers

func withUnsafePointerToVImageBuffer&lt;R>((UnsafePointer&lt;vImage_Buffer>) throws -> R) rethrows -> R

Calls the given closure with an unsafe pointer to the underlying vImage buffer.

func withUnsafeVImageBuffer&lt;R>((vImage_Buffer) throws -> R) rethrows -> R

Calls the given closure with the underlying vImage buffer.

func withUnsafeVImageBuffers&lt;R>(([vImage_Buffer]) throws -> R) rethrows -> R

Calls the given closure with the underlying vImage buffers.

### Accessing component pixel buffers

func withUnsafePixelBuffer&lt;R>(at: Int, (vImage.PixelBuffer&lt;Format.PlanarPixelFormat>) throws -> R) rethrows -> R

Calls the given closure with the pixel buffer that references the individual plane at the given index.

func withUnsafePixelBuffers&lt;R>(([vImage.PixelBuffer&lt;Format.PlanarPixelFormat>]) throws -> R) rethrows -> R

Calls the given closure with the array of pixel buffers that reference the individual planes.

## See Also

### Pixel buffer essentials

Creating vImage pixel buffers

Allocate and initialize pixel buffers from raw pixel data, Core Graphics images, and Core Video buffers.

Pixel formats

Specify a pixel buffer’s bit depth, number of channels, and data storage format.

