

- Accelerate
- vImage
- vImage.PixelBuffer
-  Convolving and applying morphology 

API Collection

# Convolving and applying morphology

Apply convolution, dilation, or erosion to a pixel buffer.

## Topics

### Morphology

func applyMorphology(operation: vImage.MorphologyOperation&lt;Pixel_8>, destination: vImage.PixelBuffer&lt;Format>)

Applies a morphology operation to an 8-bit planar pixel buffer.

func applyMorphology(operation: vImage.MorphologyOperation&lt;Pixel_F>, destination: vImage.PixelBuffer&lt;Format>)

Applies a morphology operation to a 32-bit planar pixel buffer.

func applyMorphology(operation: vImage.MorphologyOperation&lt;Pixel_8>, destination: vImage.PixelBuffer&lt;Format>)

Applies a morphology operation to an 8-bit-per-channel, 4-channel interleaved pixel buffer.

func applyMorphology(operation: vImage.MorphologyOperation&lt;Pixel_F>, destination: vImage.PixelBuffer&lt;Format>)

Applies a morphology operation to a 32-bit-per-channel, 4-channel interleaved pixel buffer.

enum MorphologyOperation

Describes which morphology operation to perform.

typealias StructuringElement

A 2D matrix that represents a morphology kernel.

### General convolution

func convolve(with: vImage.ConvolutionKernel2D&lt;Int16>, divisor: Int32?, bias: Int32?, edgeMode: vImage.EdgeMode&lt;Pixel_8>, destination: vImage.PixelBuffer&lt;Format>)

Convolves an 8-bit planar pixel buffer.

func convolve(with: vImage.ConvolutionKernel2D&lt;Float>, bias: Float?, edgeMode: vImage.EdgeMode&lt;Pixel_16F>, useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Convolves a floating-point 16-bit planar pixel buffer.

func convolve(with: vImage.ConvolutionKernel2D&lt;Float>, bias: Float?, edgeMode: vImage.EdgeMode&lt;Pixel_F>, destination: vImage.PixelBuffer&lt;Format>)

Convolves a 32-bit planar pixel buffer.

func convolve(with: vImage.ConvolutionKernel2D&lt;Int16>, divisor: Int32?, bias: Int32?, edgeMode: vImage.EdgeMode&lt;Pixel_8888>, destination: vImage.PixelBuffer&lt;Format>)

Convolves an 8-bit-per-channel, 4-channel interleaved pixel buffer.

func convolve(with: (vImage.ConvolutionKernel2D&lt;Int16>, vImage.ConvolutionKernel2D&lt;Int16>, vImage.ConvolutionKernel2D&lt;Int16>, vImage.ConvolutionKernel2D&lt;Int16>), divisors: (Int32, Int32, Int32, Int32)?, biases: (Int32, Int32, Int32, Int32), edgeMode: vImage.EdgeMode&lt;Pixel_8888>, destination: vImage.PixelBuffer&lt;Format>)

Convolves an 8-bit-per-channel, 4-channel interleaved pixel buffer with separate kernels for each channel.

func convolve(with: vImage.ConvolutionKernel2D&lt;Float>, bias: Float?, edgeMode: vImage.EdgeMode&lt;Pixel_ARGB_16F>, useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Convolves a floating-point 16-bit-per-channel, 4-channel interleaved pixel buffer.

func convolve(with: vImage.ConvolutionKernel2D&lt;Float>, bias: Float?, edgeMode: vImage.EdgeMode&lt;Pixel_FFFF>, destination: vImage.PixelBuffer&lt;Format>)

Convolves a 32-bit-per-channel, 4-channel interleaved pixel buffer.

func convolve(with: vImage.ConvolutionKernel2D&lt;Int16>, divisor: Int32?, bias: Int32?, edgeMode: vImage.EdgeMode&lt;Pixel_8>, destination: vImage.PixelBuffer&lt;Format>)

Convolves an 8-bit multiple plane pixel buffer.

func convolve(with: vImage.ConvolutionKernel2D&lt;Float>, bias: Float?, edgeMode: vImage.EdgeMode&lt;Pixel_F>, destination: vImage.PixelBuffer&lt;Format>)

Convolves a 32-bit multiple plane pixel buffer.

enum EdgeMode

Constants that specify edge modes for convolution operations.

struct ConvolutionKernel2D

A 2D matrix that represents a convolution kernel.

### Separable convolution

func separableConvolve(horizontalKernel: [Float], verticalKernel: [Float], bias: Float, edgeMode: vImage.EdgeMode&lt;Pixel_16U>, destination: vImage.PixelBuffer&lt;Format>)

Performs separable convolution on an 8-bit planar pixel buffer.

func separableConvolve(horizontalKernel: [Float], verticalKernel: [Float], bias: Float, edgeMode: vImage.EdgeMode&lt;Pixel_16F>, useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Performs separable convolution on a 16-bit planar pixel buffer.

func separableConvolve(horizontalKernel: [Float], verticalKernel: [Float], bias: Float, edgeMode: vImage.EdgeMode&lt;Pixel_F>, destination: vImage.PixelBuffer&lt;Format>)

Performs separable convolution on a 32-bit planar pixel buffer.

func separableConvolve(horizontalKernel: [Float], verticalKernel: [Float], bias: Float, edgeMode: vImage.EdgeMode&lt;Pixel_16U>, destination: vImage.PixelBuffer&lt;Format>)

Performs separable convolution on a multiple plane 8-bit pixel buffer.

func separableConvolve(horizontalKernel: [Float], verticalKernel: [Float], bias: Float, edgeMode: vImage.EdgeMode&lt;Pixel_F>, destination: vImage.PixelBuffer&lt;Format>)

Performs separable convolution on a multiple plane 32-bit pixel buffer.

struct ConvolutionKernel

Constants that describe 1D convolution kernels.

### Box convolution

func boxConvolve(kernelSize: vImage.Size, edgeMode: vImage.EdgeMode&lt;Pixel_8>, destination: vImage.PixelBuffer&lt;Format>)

Convolves an 8-bit planar pixel buffer with a box filter.

func boxConvolve(kernelSize: vImage.Size, edgeMode: vImage.EdgeMode&lt;Pixel_8888>, destination: vImage.PixelBuffer&lt;Format>)

Convolves an 8-bit-per-channel, 4-channel interleaved pixel buffer with a box filter.

func boxConvolved(kernelSize: vImage.Size, edgeMode: vImage.EdgeMode&lt;Pixel_8888>) -> vImage.PixelBuffer&lt;Format>

Returns a box-filter convolved 8-bit-per-channel, 4-channel interleaved pixel buffer.

func boxConvolve(kernelSize: vImage.Size, edgeMode: vImage.EdgeMode&lt;Pixel_8>, destination: vImage.PixelBuffer&lt;Format>)

Convolves a multiple-plane 8-bit-per-channel pixel buffer with a box filter.

### Tent convolution

func tentConvolve(kernelSize: vImage.Size, edgeMode: vImage.EdgeMode&lt;Pixel_8>, destination: vImage.PixelBuffer&lt;Format>)

Convolves an 8-bit planar pixel buffer with a tent filter.

func tentConvolve(kernelSize: vImage.Size, edgeMode: vImage.EdgeMode&lt;Pixel_8888>, destination: vImage.PixelBuffer&lt;Format>)

Convolves an 8-bit-per-channel, 4-channel interleaved pixel buffer with a tent filter.

func tentConvolved(kernelSize: vImage.Size, edgeMode: vImage.EdgeMode&lt;Pixel_8888>) -> vImage.PixelBuffer&lt;Format>

Returns a tent-filter convolved 8-bit-per-channel, 4-channel interleaved pixel buffer.

func tentConvolve(kernelSize: vImage.Size, edgeMode: vImage.EdgeMode&lt;Pixel_8>, destination: vImage.PixelBuffer&lt;Format>)

Convolves a multiple-plane 8-bit-per-channel pixel buffer with a tent filter.

## See Also

### Pixel buffer operations

Applying geometric operations to pixel buffers

Reflect, shear, rotate, scale, and apply affine transforms to image data.

Applying color transforms to pixel buffers

Adjust the colors of an image by applying gamma, polynomials, or multidimensional lookup.

Blending and compositing pixel buffers

Composite two pixel buffers to create a single image.

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

