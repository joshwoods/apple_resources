

- Accelerate
- vImage
- vImage.PixelBuffer
-  Blending and compositing pixel buffers 

API Collection

# Blending and compositing pixel buffers

Composite two pixel buffers to create a single image.

## Topics

### Alpha compositing

func alphaComposite(vImage.CompositeMode&lt;Pixel_8>, topLayer: vImage.PixelBuffer&lt;Format>, destination: vImage.PixelBuffer&lt;Format>)

Performs alpha compositing of two 4-channel interleaved ARGB 8-bit pixel buffers using the specified composite mode.

func alphaComposite(vImage.CompositeMode&lt;Pixel_F>, topLayer: vImage.PixelBuffer&lt;Format>, destination: vImage.PixelBuffer&lt;Format>)

Performs alpha compositing of two 4-channel interleaved ARGB 32-bit pixel buffers using the specified composite mode.

enum CompositeMode

Constants that specify whether the format of layers is premultiplied or nonpremultiplied.

### Alpha blending

func premultipliedAlphaBlend(vImage.BlendMode, topLayer: vImage.PixelBuffer&lt;Format>, destination: vImage.PixelBuffer&lt;Format>)

Performs alpha compositing of two 4-channel interleaved RGBA 8-bit pixel buffers using the specified blend mode to produce a premultiplied result.

enum BlendMode

Constants that specify an alpha blending mode.

### Premultiply

func premultiply(alpha: vImage.PixelBuffer&lt;Format>)

Transforms an 8-bit planar pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

func premultiply(alpha: vImage.PixelBuffer&lt;Format>)

Transforms a 32-bit planar pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

func premultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an 8-bit ARGB or RGBA pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

func premultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an unsigned 16-bit ARGB or RGBA pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

func premultiply()

Transforms a floating-point 16-bit RGBA pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

func premultiply(channelOrdering: vImage.ChannelOrdering)

Transforms a floating-point 32-bit ARGB or RGBA pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

### Unpremultiply

func unpremultiply(alpha: vImage.PixelBuffer&lt;Format>)

Transforms an 8-bit planar pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(alpha: vImage.PixelBuffer&lt;Format>)

Transforms a 32-bit planar pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an 8-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an unsigned 16-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply()

Transforms a floating-point 16-bit RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms a 32-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

### Linear interpolation

func linearInterpolate(bufferB: vImage.PixelBuffer&lt;Format>, interpolationConstant: Float, destination: vImage.PixelBuffer&lt;Format>)

## See Also

### Pixel buffer operations

Applying geometric operations to pixel buffers

Reflect, shear, rotate, scale, and apply affine transforms to image data.

Applying color transforms to pixel buffers

Adjust the colors of an image by applying gamma, polynomials, or multidimensional lookup.

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

Applying channel operations

Extract, flatten, permute, and overwrite the individual color channels of a pixel buffer.

Applying arithmetic operations

Multiply the pixel values of a buffer by scalar values or matrices.

