

- Accelerate
- vImage
- vImage.PixelBuffer
-  Converting pixel buffers 

API Collection

# Converting pixel buffers

Convert pixel buffer data between different bit-depths.

## Topics

### Conversion from YUV to RGB

func convert(lumaSource: vImage.PixelBuffer&lt;vImage.Planar8>, chromaSource: vImage.PixelBuffer&lt;vImage.Interleaved8x2>, conversionInfo: vImage_YpCbCrToARGB)

Populates the pixel buffer with ARGB data from the given luminance and chrominance pixel buffers.

### Conversion from 8-bit to 16-bit

func convert(to: vImage.PixelBuffer&lt;vImage.Planar16F>)

Converts the contents of the 8-bit planar pixel buffer to floating-point 16-bit planar format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved16Fx2>)

Converts the contents of the 8-bit-per-channel, 2-channel interleaved pixel buffer to floating-point 16-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved16Ux4>)

Converts the contents of the 8-bit-per-channel, 4-channel interleaved pixel buffer to unsigned 16-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved16Fx4>)

Converts the contents of the 8-bit-per-channel, 4-channel interleaved pixel buffer to floating-point 16-bit-per-channel format.

### Conversion from 8-bit to 32-bit

func convert(to: vImage.PixelBuffer&lt;vImage.PlanarF>)

Converts the contents of the 8-bit planar pixel buffer to 32-bit planar format.

func convert(to: vImage.PixelBuffer&lt;vImage.InterleavedFx3>)

Converts the contents of the 8-bit-per-channel, 3-channel interleaved pixel buffer to 32-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Converts the contents of the 8-bit-per-channel, 4-channel interleaved pixel buffer to 32-bit-per-channel format.

### Conversion from 16-bit to 8-bit

func convert(to: vImage.PixelBuffer&lt;vImage.Planar8>)

Converts the contents of the floating-point 16-bit planar pixel buffer to 8-bit planar format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved8x2>)

Converts the contents of the floating-point 16-bit-per-channel, 2-channel interleaved pixel buffer to 8-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Converts the contents of the unsigned 16-bit-per-channel, 4-channel interleaved pixel buffer to 8-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Converts the contents of the floating-point 16-bit-per-channel, 4-channel interleaved pixel buffer to 8-bit-per-channel format.

### Conversion between 16-bit formats

func convert(to: vImage.PixelBuffer&lt;vImage.Planar16F>)

Converts the contents of the unsigned 16-bit planar pixel buffer to floating-point 16-bit planar format.

func convert(to: vImage.PixelBuffer&lt;vImage.Planar16U>)

Converts the contents of the floating-point 16-bit planar pixel buffer to unsigned 16-bit planar format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved16Ux2>)

Converts the contents of the floating-point 16-bit-per-channel, 2-channel interleaved pixel buffer to unsigned 16-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved16Fx4>)

Converts the contents of the unsigned 16-bit-per-channel, 4-channel interleaved pixel buffer to floating-point 16-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved16Ux4>)

Converts the contents of the floating-point 16-bit-per-channel, 4-channel interleaved pixel buffer to unsigned 16-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved16Fx2>)

Converts the contents of the unsigned 16-bit-per-channel, 2-channel interleaved pixel buffer to floating-point 16-bit-per-channel format.

### Conversion from 16-bit to 32-bit

func convert(to: vImage.PixelBuffer&lt;vImage.PlanarF>)

Converts the contents of the floating-point 16-bit planar pixel buffer to 32-bit planar format.

func convert(to: vImage.PixelBuffer&lt;vImage.InterleavedFx2>)

Converts the contents of the floating-point 16-bit-per-channel, 2-channel interleaved pixel buffer to 32-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Converts the contents of the unsigned 16-bit-per-channel, 4-channel interleaved pixel buffer to 32-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Converts the contents of the floating-point 16-bit-per-channel, 4-channel interleaved pixel buffer to 32-bit-per-channel format.

### Conversion from 32-bit to 8-bit

func convert(to: vImage.PixelBuffer&lt;vImage.Planar8>)

Converts the contents of the 32-bit planar pixel buffer to 8-bit planar format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved8x3>)

Converts the contents of the 32-bit-per-channel, 3-channel interleaved pixel buffer to 8-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Converts the contents of the 32-bit-per-channel, 4-channel interleaved pixel buffer to 8-bit-per-channel format.

### Conversion from 32-bit to 16-bit

func convert(to: vImage.PixelBuffer&lt;vImage.Planar16F>)

Converts the contents of the 32-bit planar pixel buffer to floating-point 16-bit planar format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved16Fx2>)

Converts the contents of the 32-bit-per-channel, 2-channel interleaved pixel buffer to floating-point 16-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved16Fx4>)

Converts the contents of the 32-bit-per-channel, 4-channel interleaved pixel buffer to floating-point 16-bit-per-channel format.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved16Ux4>)

Converts the contents of the 32-bit-per-channel, 4-channel interleaved pixel buffer to unsigned 16-bit-per-channel format.

### Conversion from four channels to three channels

func convert(to: vImage.PixelBuffer&lt;vImage.InterleavedFx3>, channelOrdering: vImage.ChannelOrdering)

Converts the 32-bit-per-channel RGBA or ARGB pixel buffer to RGB.

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved8x3>, channelOrdering: vImage.ChannelOrdering)

Converts the 8-bit-per-channel RGBA or ARGB pixel buffer to RGB.

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

Interleaving and deinterleaving pixel buffers

Convert pixel buffer data between interleaved and planar formats.

Cropping and working with regions of interest

Crop images and apply operations to regions of interest.

Applying channel operations

Extract, flatten, permute, and overwrite the individual color channels of a pixel buffer.

Applying arithmetic operations

Multiply the pixel values of a buffer by scalar values or matrices.

