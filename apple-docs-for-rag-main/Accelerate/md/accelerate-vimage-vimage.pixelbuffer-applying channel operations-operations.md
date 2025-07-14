

- Accelerate
- vImage
- vImage.PixelBuffer
-  Applying channel operations 

API Collection

# Applying channel operations

Extract, flatten, permute, and overwrite the individual color channels of a pixel buffer.

## Topics

### Extracting Channels

func extractChannel(at: Int, destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Extracts a single channel from an 8-bit-per-channel, 4-channel interleaved pixel buffer.

func extractChannel(at: Int, destination: vImage.PixelBuffer&lt;vImage.Planar16U>)

Extracts a single channel from an unsigned 16-bit-per-channel, 4-channel interleaved pixel buffer.

func extractChannel(at: Int, destination: vImage.PixelBuffer&lt;vImage.PlanarF>)

Extracts a single channel from an 32-bit-per-channel, 4-channel interleaved pixel buffer.

### Flattening Channels

func flatten(channelOrdering: vImage.ChannelOrdering, backgroundColor: Pixel_8888, isPremultiplied: Bool, destination: vImage.PixelBuffer&lt;vImage.Interleaved8x3>)

Transforms an 8-bit-per-channel RGBA or ARGB buffer to an RGB buffer against an opaque background color.

func flatten(channelOrdering: vImage.ChannelOrdering, backgroundColor: Pixel_FFFF, isPremultiplied: Bool, destination: vImage.PixelBuffer&lt;vImage.InterleavedFx3>)

Transforms an 32-bit-per-channel RGBA or ARGB buffer to an RGB buffer against an opaque background color.

enum ChannelOrdering

Constants that specify the channel ordering of a pixel buffer.

### Permuting Channels

func permuteChannels(to: (UInt8, UInt8, UInt8), destination: vImage.PixelBuffer&lt;Format>)

Permutes the channels of an 8-bit-per-channel, 3-channel interleaved pixel buffer.

func permuteChannels(to: (UInt8, UInt8, UInt8, UInt8), destination: vImage.PixelBuffer&lt;Format>)

Permutes the channels of an 8-bit-per-channel, 4-channel interleaved pixel buffer.

func permuteChannels(to: (UInt8, UInt8, UInt8, UInt8), destination: vImage.PixelBuffer&lt;Format>)

Permutes the channels of an unsigned 16-bit-per-channel, 4-channel interleaved pixel buffer.

func permuteChannels(to: (UInt8, UInt8, UInt8, UInt8), destination: vImage.PixelBuffer&lt;Format>)

Permutes the channels of a floating-point 16-bit-per-channel, 4-channel interleaved pixel buffer.

func permuteChannels(to: (UInt8, UInt8, UInt8, UInt8), destination: vImage.PixelBuffer&lt;Format>)

Permutes the channels of an 32-bit-per-channel, 4-channel interleaved pixel buffer.

### Overwriting Channels

func overwriteChannels(withScalar: Pixel_8)

Overwrites the pixels of the pixel buffer with the provided 8-bit scalar value.

func overwriteChannels(withScalar: Pixel_16F)

Overwrites the pixels of the pixel buffer with the provided floating-point 16-bit scalar value.

func overwriteChannels(withScalar: Pixel_F)

Overwrites the pixels of the pixel buffer with the provided 32-bit scalar value.

func overwriteChannels([UInt8], withScalar: Pixel_8, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 8-bit scalar value.

func overwriteChannels([UInt8], withScalar: Pixel_F, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 32-bit scalar value.

func overwriteChannels([UInt8], withPixel: Pixel_8888, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 8-bit, 4-channel pixel value.

func overwriteChannels([UInt8], withPixel: Pixel_ARGB_16U, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided unsigned 16-bit, 4-channel pixel value.

func overwriteChannels([UInt8], withPixel: Pixel_FFFF, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 32-bit, 4-channel pixel value.

func overwriteChannels([UInt8], withPlanarBuffer: vImage.PixelBuffer&lt;vImage.Planar8>, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 8-bit planar pixel buffer.

func overwriteChannels([UInt8], withPlanarBuffer: vImage.PixelBuffer&lt;vImage.PlanarF>, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 32-bit planar pixel buffer.

func overwriteChannels([UInt8], withInterleavedBuffer: vImage.PixelBuffer&lt;Format>, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 8-bit interleaved pixel buffer.

func overwriteChannels([UInt8], withInterleavedBuffer: vImage.PixelBuffer&lt;Format>, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 32-bit interleaved pixel buffer.

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

Interleaving and deinterleaving pixel buffers

Convert pixel buffer data between interleaved and planar formats.

Cropping and working with regions of interest

Crop images and apply operations to regions of interest.

Applying arithmetic operations

Multiply the pixel values of a buffer by scalar values or matrices.

