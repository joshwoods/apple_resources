

- Accelerate
- vImage
- vImage.PixelBuffer
-  Cropping and working with regions of interest 

API Collection

# Cropping and working with regions of interest

Crop images and apply operations to regions of interest.

## Topics

### Cropping

func crop(at: CGPoint, destination: vImage.PixelBuffer&lt;Format>)

Crops the pixel buffer to a rectangle that’s defined by an origin and the destination buffer’s dimensions.

func cropped(to: CGRect) -> vImage.PixelBuffer&lt;Format>

Returns a new pixel buffer that contains a copy of the data specified as a subregion of an existing pixel buffer.

### Region of Interest

func withUnsafeRegionOfInterest&lt;R>(CGRect, (vImage.PixelBuffer&lt;Format>) throws -> R) rethrows -> R

Calls the given closure with a pixel buffer that references the image data within the specified region of interest.

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

Applying channel operations

Extract, flatten, permute, and overwrite the individual color channels of a pixel buffer.

Applying arithmetic operations

Multiply the pixel values of a buffer by scalar values or matrices.

