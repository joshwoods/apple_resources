

- Accelerate
- vImage
- vImage.PixelBuffer
-  Applying color transforms to pixel buffers 

API Collection

# Applying color transforms to pixel buffers

Adjust the colors of an image by applying gamma, polynomials, or multidimensional lookup.

## Topics

### Applying gamma

func applyGamma(vImage.Gamma, intermediateBuffer: vImage.PixelBuffer&lt;vImage.PlanarF>?, destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Applies a gamma function to an 8-bit planar pixel buffer.

func applyGamma(vImage.Gamma, intermediateBuffer: vImage.PixelBuffer&lt;vImage.InterleavedFx2>?, destination: vImage.PixelBuffer&lt;vImage.Interleaved8x2>)

Applies a gamma function to an 8-bit-per-channel, 2-channel interleaved pixel buffer.

func applyGamma(vImage.Gamma, intermediateBuffer: vImage.PixelBuffer&lt;vImage.InterleavedFx3>?, destination: vImage.PixelBuffer&lt;vImage.Interleaved8x3>)

Applies a gamma function to an 8-bit-per-channel, 3-channel interleaved pixel buffer.

func applyGamma(vImage.Gamma, intermediateBuffer: vImage.PixelBuffer&lt;vImage.InterleavedFx4>?, destination: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Applies a gamma function to an 8-bit-per-channel, 4-channel interleaved pixel buffer.

func applyGamma(vImage.Gamma, destination: vImage.PixelBuffer&lt;Format>)

Applies a gamma function to a 32-bit pixel buffer.

enum Gamma

Describes either a used-defined or constant gamma.

### Applying piecewise gamma

func applyGamma(linearParameters: (scale: Float, bias: Float), exponentialParameters: (scale: Float, preBias: Float, gamma: Float, postBias: Float), boundary: Pixel_8, destination: vImage.PixelBuffer&lt;Format>)

Applies a piecewise gamma calculation to an 8-bit pixel buffer.

func applyGamma(linearParameters: (scale: Float, bias: Float), exponentialParameters: (scale: Float, preBias: Float, gamma: Float, postBias: Float), boundary: Float, destination: vImage.PixelBuffer&lt;Format>)

Applies a piecewise gamma calculation to a 32-bit pixel buffer.

### Appying polynomial (32-bit source, 8-bit destination)

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Applies a set of piecewise polynomials to a 32-bit planar buffer and writes the result to an 8-bit planar buffer.

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;vImage.Interleaved8x2>)

Applies a set of piecewise polynomials to a 2-channel, 32-bit interleaved buffer and writes the result to a 2-channel, 8-bit interleaved buffer.

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;vImage.Interleaved8x3>)

Applies a set of piecewise polynomials to a 3-channel, 32-bit interleaved buffer and writes the result to a 3-channel, 8-bit interleaved buffer.

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Applies a set of piecewise polynomials to a 4-channel, 32-bit interleaved buffer and writes the result to a 4-channel, 8-bit interleaved buffer.

### Appying polynomial (8-bit source, 32-bit destination)

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;vImage.PlanarF>)

Applies a set of piecewise polynomials to an 8-bit planar buffer and writes the result to a 32-bit planar buffer.

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;vImage.InterleavedFx2>)

Applies a set of piecewise polynomials to a 2-channel, 8-bit interleaved buffer and writes the result to a 2-channel, 32-bit interleaved buffer.

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;vImage.InterleavedFx3>)

Applies a set of piecewise polynomials to a 3-channel, 8-bit interleaved buffer and writes the result to a 3-channel, 32-bit interleaved buffer.

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Applies a set of piecewise polynomials to a 4-channel, 8-bit interleaved buffer and writes the result to a 4-channel, 32-bit interleaved buffer.

### Appying polynomial (32-bit)

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;Format>)

Applies a set of piecewise polynomials to a 32-bit planar buffer.

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;Format>)

Applies a set of piecewise polynomials to a 2-channel, 32-bit interleaved buffer.

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;Format>)

Applies a set of piecewise polynomials to a 3-channel, 32-bit interleaved buffer.

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;Format>)

Applies a set of piecewise polynomials to a 4-channel, 32-bit interleaved buffer.

### Transforming with a lookup table

func applyLookup([Pixel_8], destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Applies a lookup table to transform an 8-bit planar image.

func applyLookup([Pixel_F], destination: vImage.PixelBuffer&lt;vImage.PlanarF>)

Applies a lookup table to transform an 8-bit planar image to a 32-bit planar image.

func applyLookup([Pixel_16U], destination: vImage.PixelBuffer&lt;vImage.Planar16U>)

Applies a lookup table to transform an 8-bit planar image to a 16-bit planar image.

func applyLookup([Pixel_8888], destination: vImage.PixelBuffer&lt;vImage.Interleaved8x3>)

Applies a lookup table to transform an 8-bit planar image to an 8-bit-per-channel, three-channel interleaved image.

func applyLookup([Pixel_FFFF], destination: vImage.PixelBuffer&lt;vImage.InterleavedFx3>)

Applies a lookup table to transform an 8-bit planar image to a 32-bit-per-channel, three-channel interleaved image.

func applyLookup(alphaTable: [Pixel_8]?, redTable: [Pixel_8]?, greenTable: [Pixel_8]?, blueTable: [Pixel_8]?, destination: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Applies a set of four lookup tables to transform an interleaved, four-channel 8-bit image.

### Transforming with a multidimensional lookup table

struct MultidimensionalLookupTable

A multidimensional lookup table.

### Applying a flood fill to an image

func floodFill(from: CGPoint, newColor: Pixel_8, connectivity: vImage.FloodFillConnectivity)

Applies an in-place flood-fill operation to the 8-bit planar image.

func floodFill(from: CGPoint, newColor: Pixel_8888, connectivity: vImage.FloodFillConnectivity)

Applies an in-place flood-fill operation to the interleaved 4-channel, 8-bit-per-pixel image.

func floodFill(from: CGPoint, newColor: Pixel_16U, connectivity: vImage.FloodFillConnectivity)

Applies an in-place flood-fill operation to the unsigned 16-bit planar image.

func floodFill(from: CGPoint, newColor: Pixel_ARGB_16U, connectivity: vImage.FloodFillConnectivity)

Applies an in-place flood-fill operation to the interleaved 4-channel, unsigned16-bit-per-pixel image.

## See Also

### Pixel buffer operations

Applying geometric operations to pixel buffers

Reflect, shear, rotate, scale, and apply affine transforms to image data.

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

Applying arithmetic operations

Multiply the pixel values of a buffer by scalar values or matrices.

