

- Accelerate
- vImage
- vImage.PixelBuffer
-  Applying arithmetic operations 

API Collection

# Applying arithmetic operations

Multiply the pixel values of a buffer by scalar values or matrices.

## Topics

### Scalar Multiplication

func multiply(by: Int, divisor: Int, preBias: Int, postBias: Int, destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Multiplies each pixel in an 8-bit planar pixel buffer by the specified factor.

func multiply(by: Float, preBias: Float, postBias: Float, destination: vImage.PixelBuffer&lt;vImage.PlanarF>)

Multiplies each pixel in a 32-bit planar pixel buffer by the specified factor.

### Matrix Multiplication

func multiply&lt;Matrix>(by: Matrix, divisor: Int, preBias: (Int, Int, Int, Int), postBias: (Int, Int, Int, Int), destination: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Multiplies each four channel pixel in an 8-bit-per channel, 4-channel pixel buffer by a 4 x 4 matrix to produce a four channel result.

func multiply&lt;Matrix>(by: Matrix, preBias: (Float, Float, Float, Float), postBias: (Float, Float, Float, Float), destination: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Multiplies each four channel pixel in a 32-bit-per channel, 4-channel pixel buffer by a 4 x 4 matrix to produce a four channel result.

func multiply(by: simd_float4x4, preBias: (Float, Float, Float, Float), postBias: (Float, Float, Float, Float), destination: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Multiplies each four channel pixel in a 32-bit-per channel, 4-channel pixel buffer by a 4 x 4 simd matrix to produce a four channel result.

func multiply&lt;Matrix, DestFormat>(by: Matrix, divisor: Int, preBias: [Int], postBias: [Int], destination: vImage.PixelBuffer&lt;DestFormat>)

Multiplies each four channel pixel in an 8-bit multiple-plane pixel buffer by a 4 x 4 matrix to produce a four channel result.

func multiply&lt;Matrix, DestFormat>(by: Matrix, preBias: [Float], postBias: [Float], destination: vImage.PixelBuffer&lt;DestFormat>)

Multiplies each four channel pixel in a 32-bit multiple-plane pixel buffer by a 4 x 4 matrix to produce a four channel result.

### Pixel Multiplication

func multiply(by: (Int, Int, Int, Int), divisor: Int, preBias: (Int, Int, Int, Int), postBias: Int, destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Multiplies each four channel pixel in an 8-bit-per channel, 4-channel pixel buffer by a four element matrix to produce a single channel result.

func multiply(by: (Float, Float, Float, Float), preBias: (Float, Float, Float, Float), postBias: Float, destination: vImage.PixelBuffer&lt;vImage.PlanarF>)

Multiplies each four channel pixel in a 32-bit-per channel, 4-channel pixel buffer by a four element matrix to produce a single channel result.

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

Applying channel operations

Extract, flatten, permute, and overwrite the individual color channels of a pixel buffer.

