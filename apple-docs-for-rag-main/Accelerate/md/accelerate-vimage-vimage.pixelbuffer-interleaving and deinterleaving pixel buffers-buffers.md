

- Accelerate
- vImage
- vImage.PixelBuffer
-  Interleaving and deinterleaving pixel buffers 

API Collection

# Interleaving and deinterleaving pixel buffers

Convert pixel buffer data between interleaved and planar formats.

## Topics

### Deinterleaving pixel buffers

func deinterleave(destination: vImage.PixelBuffer&lt;vImage.Planar8x3>)

Deinterleaves the 8-bit-per-channel, three-channel interleaved buffer and writes the result to a multiple-plane pixel buffer.

func deinterleave(destination: vImage.PixelBuffer&lt;vImage.Planar8x4>)

Deinterleaves the 8-bit-per-channel, four-channel interleaved buffer and writes the result to a multiple-plane pixel buffer.

func deinterleave(destination: vImage.PixelBuffer&lt;vImage.PlanarFx3>)

Deinterleaves the 32-bit-per-channel, three-channel interleaved buffer and writes the result to a multiple-plane pixel buffer.

func deinterleave(destination: vImage.PixelBuffer&lt;vImage.PlanarFx4>)

Deinterleaves the 32-bit-per-channel, four-channel interleaved buffer and writes the result to a multiple-plane pixel buffer.

func deinterleave(planarDestinationBuffers: [vImage.PixelBuffer&lt;vImage.Planar8>])

Deinterleaves the 8-bit-per-channel, three-channel interleaved buffer and writes the result to an array that contains three planar buffers.

func deinterleave(planarDestinationBuffers: [vImage.PixelBuffer&lt;vImage.Planar8>])

Deinterleaves the 8-bit-per-channel, four-channel interleaved buffer and writes the result to an array that contains four planar buffers.

func deinterleave(planarDestinationBuffers: [vImage.PixelBuffer&lt;vImage.Planar16F>])

Deinterleaves the 16-bit-per-channel, four-channel interleaved buffer and writes the result to an array that contains four planar buffers.

func deinterleave(planarDestinationBuffers: [vImage.PixelBuffer&lt;vImage.Planar16U>])

Deinterleaves the unsigned 16-bit-per-channel, four-channel interleaved buffer and writes the result to an array that contains four planar buffers.

func deinterleave(planarDestinationBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Deinterleaves the 32-bit-per-channel, three-channel interleaved buffer and writes the result to an array that contains three planar buffers.

func deinterleave(planarDestinationBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Deinterleaves the 32-bit-per-channel, four-channel interleaved buffer and writes the result to an array that contains four planar buffers.

### Interleaving pixel buffers

func interleave(destination: vImage.PixelBuffer&lt;vImage.Interleaved8x3>)

Interleaves the 8-bit-per-channel, three-channel multiple-plane buffer and writes the result to an interleaved pixel buffer.

func interleave(destination: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Interleaves the 8-bit-per-channel, four-channel multiple-plane buffer and writes the result to an interleaved pixel buffer.

func interleave(destination: vImage.PixelBuffer&lt;vImage.InterleavedFx3>)

Interleaves the 32-bit-per-channel, three-channel multiple-plane buffer and writes the result to an interleaved pixel buffer.

func interleave(destination: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Interleaves the 32-bit-per-channel, four-channel multiple-plane buffer and writes the result to an interleaved pixel buffer.

func interleave(planarSourceBuffers: [vImage.PixelBuffer&lt;vImage.Planar8>])

Interleaves the specified planar source buffers and writes the result to the 8-bit-per-channel, three-channel interleaved buffer.

func interleave(planarSourceBuffers: [vImage.PixelBuffer&lt;vImage.Planar8>])

Interleaves the specified planar source buffers and writes the result to the 8-bit-per-channel, four-channel interleaved buffer.

func interleave(planarSourceBuffers: [vImage.PixelBuffer&lt;vImage.Planar16F>])

Interleaves the specified planar source buffers and writes the result to the 16-bit-per-channel, four-channel interleaved buffer.

func interleave(planarSourceBuffers: [vImage.PixelBuffer&lt;vImage.Planar16U>])

Interleaves the specified planar source buffers and writes the result to the unsigned 16-bit-per-channel, four-channel interleaved buffer.

func interleave(planarSourceBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Interleaves the specified planar source buffers and writes the result to the 32-bit-per-channel, three-channel interleaved buffer.

func interleave(planarSourceBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Interleaves the specified planar source buffers and writes the result to the 32-bit-per-channel, four-channel interleaved buffer.

### Generating planar buffers from interleaved buffers

func planarBuffers() -> [vImage.PixelBuffer&lt;vImage.Planar8>]

Returns two 8-bit planar pixel buffers that contain the deinterleaved channels of the buffer.

func planarBuffers() -> [vImage.PixelBuffer&lt;vImage.Planar8>]

Returns three 8-bit planar pixel buffers that contain the deinterleaved channels of the buffer.

func planarBuffers() -> [vImage.PixelBuffer&lt;vImage.Planar8>]

Returns four 8-bit planar pixel buffers that contain the deinterleaved channels of the buffer.

func planarBuffers() -> [vImage.PixelBuffer&lt;vImage.PlanarF>]

Returns four 32-bit planar pixel buffers that contain the deinterleaved channels of the 8-bit buffer.

func planarBuffers() -> [vImage.PixelBuffer&lt;vImage.Planar16U>]

Returns four unsigned 16-bit planar pixel buffers that contain the deinterleaved channels of the buffer.

func planarBuffers() -> [vImage.PixelBuffer&lt;vImage.PlanarF>]

Returns two 32-bit planar pixel buffers that contain the deinterleaved channels of the buffer.

func planarBuffers() -> [vImage.PixelBuffer&lt;vImage.PlanarF>]

Returns three 32-bit planar pixel buffers that contain the deinterleaved channels of the buffer.

func planarBuffers() -> [vImage.PixelBuffer&lt;vImage.Planar8>]

Returns four 8-bit planar pixel buffers that contain the deinterleaved channels of the 32-bit buffer.

func planarBuffers() -> [vImage.PixelBuffer&lt;vImage.PlanarF>]

Returns four 32-bit planar pixel buffers that contain the deinterleaved channels of the buffer.

### Converting from 8-bit multiple plane to 8-bit interleaved

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved8x3>)

Converts the contents of an 8-bit, three-plane pixel buffer to a three-channel interleaved pixel buffer.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Converts the contents of an 8-bit, four-plane pixel buffer to a four-channel interleaved pixel buffer.

### Converting from 32-bit multiple plane to 32-bit interleaved

func convert(to: vImage.PixelBuffer&lt;vImage.InterleavedFx3>)

Converts the contents of a 32-bit, three-plane pixel buffer to a three-channel interleaved pixel buffer.

func convert(to: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Converts the contents of a 32-bit, four-plane pixel buffer to a four-channel interleaved pixel buffer.

## See Also

### Pixel buffer operations

Applying geometric operations to pixel buffers

Reflect, shear, rotate, scale, and apply affine transforms to image data.

Applying color transforms to pixel buffers

Adjust the colors of an image by applying gamma, polynomials, or multidimensional lookup.

Blending and compositing pixel buffers

Composite two pixel buffers to create a single image.

Convolving and applying morphology

Apply convolution, dilation, or erosion to a pixel buffer.

Thresholding and clipping pixel buffer values

Limit the values in a pixel buffer to a threshold or a range.

Calculating and transforming histograms

Enhance and adjust the contrast of an image with histogram equalization, contrast stretching, and specification.

Converting pixel buffers

Convert pixel buffer data between different bit-depths.

Cropping and working with regions of interest

Crop images and apply operations to regions of interest.

Applying channel operations

Extract, flatten, permute, and overwrite the individual color channels of a pixel buffer.

Applying arithmetic operations

Multiply the pixel values of a buffer by scalar values or matrices.

