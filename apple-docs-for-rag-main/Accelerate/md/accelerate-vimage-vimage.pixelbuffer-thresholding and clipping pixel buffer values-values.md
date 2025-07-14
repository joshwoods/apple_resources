

- Accelerate
- vImage
- vImage.PixelBuffer
-  Thresholding and clipping pixel buffer values 

API Collection

# Thresholding and clipping pixel buffer values

Limit the values in a pixel buffer to a threshold or a range.

## Topics

### Clipping

func clip(to: ClosedRange&lt;Float>, destination: vImage.PixelBuffer&lt;Format>)

Clips the values of a 32-bit pixel buffer to the specified bounds.

### Threshold

func colorThreshold(Float, destination: vImage.PixelBuffer&lt;Format>)

Creates a binary image from a 32-bit pixel buffer.

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

