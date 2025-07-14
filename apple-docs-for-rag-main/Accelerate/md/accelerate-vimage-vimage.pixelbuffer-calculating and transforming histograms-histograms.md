

- Accelerate
- vImage
- vImage.PixelBuffer
-  Calculating and transforming histograms 

API Collection

# Calculating and transforming histograms

Enhance and adjust the contrast of an image with histogram equalization, contrast stretching, and specification.

## Topics

### Contrast stretching

func contrastStretch(destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Stretches the histogram of an 8-bit planar pixel buffer.

func contrastStretch(binCount: Int, destination: vImage.PixelBuffer&lt;vImage.PlanarF>)

Stretches the histogram of a 32-bit planar pixel buffer.

func contrastStretch(destination: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Stretches the histogram of an 8-bit-per-channel, 4-channel interleaved pixel buffer.

func contrastStretch(binCount: Int, destination: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Stretches the histogram of a 32-bit-per-channel, 4-channel interleaved pixel buffer.

func contrastStretch(destination: vImage.PixelBuffer&lt;Format>)

Stretches the histogram of a multiple-plane 8-bit pixel buffer.

func contrastStretch(binCount: Int, destination: vImage.PixelBuffer&lt;Format>)

Stretches the histogram of a multiple-plane 32-bit pixel buffer.

### Equalization

func equalizeHistogram(destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Equalizes the histogram of an 8-bit planar pixel buffer.

func equalizeHistogram(binCount: Int, destination: vImage.PixelBuffer&lt;vImage.PlanarF>)

Equalizes the histogram of a 32-bit planar pixel buffer.

func equalizeHistogram(destination: vImage.PixelBuffer&lt;Format>)

Equalizes the histogram of an 8-bit-per-channel, 4-channel interleaved pixel buffer.

func equalizeHistogram(binCount: Int, destination: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Equalizes the histogram of a 32-bit-per-channel, 4-channel interleaved pixel buffer.

func equalizeHistogram(destination: vImage.PixelBuffer&lt;Format>)

Equalizes the histogram of a multiple-plane 8-bit pixel buffer.

func equalizeHistogram(binCount: Int, destination: vImage.PixelBuffer&lt;Format>)

Equalizes the histogram of a multiple-plane 32-bit pixel buffer.

### Histogram calculation

func histogram() -> vImage.PixelBuffer&lt;Format>.Histogram8888

Calculates the histogram of an 8-bit-per-channel, 4-channel interleaved pixel buffer.

func histogram(binCount: Int) -> vImage.PixelBuffer&lt;Format>.HistogramFFFF

Calculates the histogram of a 32-bit-per-channel, 4-channel interleaved pixel buffer.

func histogram() -> vImage.PixelBuffer&lt;Format>.Histogram888

Calculates the histogram of an 8-bit-per-channel, 3-channel multiple-plane pixel buffer.

func histogram(binCount: Int) -> vImage.PixelBuffer&lt;Format>.HistogramFFF

Calculates the histogram of a 32-bit-per-channel, 3-channel multiple-plane pixel buffer.

func histogram() -> vImage.PixelBuffer&lt;Format>.Histogram8888

Calculates the histogram of an 8-bit-per-channel, 4-channel multiple-plane pixel buffer.

func histogram(binCount: Int) -> vImage.PixelBuffer&lt;Format>.HistogramFFFF

Calculates the histogram of a 32-bit-per-channel, 4-channel multiple-plane pixel buffer.

### Histogram specification

func specifyHistogram(vImage.PixelBuffer&lt;Format>.Histogram8888, destination: vImage.PixelBuffer&lt;Format>)

Performs a histogram specification operation on an 8-bit-per-channel, 4-channel interleaved pixel buffer.

func specifyHistogram(vImage.PixelBuffer&lt;Format>.HistogramFFFF, destination: vImage.PixelBuffer&lt;Format>)

Performs a histogram specification operation on a 32-bit-per-channel, 4-channel interleaved pixel buffer.

func specifyHistogram(vImage.PixelBuffer&lt;Format>.Histogram888, destination: vImage.PixelBuffer&lt;Format>)

Performs a histogram specification operation on an 8-bit-per-channel, 3-channel multiple-plane pixel buffer.

func specifyHistogram(vImage.PixelBuffer&lt;Format>.HistogramFFF, destination: vImage.PixelBuffer&lt;Format>)

Performs a histogram specification operation on a 32-bit-per-channel, 3-channel multiple-plane pixel buffer.

func specifyHistogram(vImage.PixelBuffer&lt;Format>.Histogram8888, destination: vImage.PixelBuffer&lt;Format>)

Performs a histogram specification operation on an 8-bit-per-channel, 4-channel multiple-plane pixel buffer.

func specifyHistogram(vImage.PixelBuffer&lt;Format>.HistogramFFFF, destination: vImage.PixelBuffer&lt;Format>)

Performs a histogram specification operation on a 32-bit-per-channel, 3-channel multiple-plane pixel buffer.

### Type aliases

typealias Histogram888

The histogram for three channel 8-bit pixel buffers.

typealias Histogram8888

The histogram for four channel 8-bit pixel buffers.

typealias HistogramFFF

The histogram for three channel 32-bit pixel buffers.

typealias HistogramFFFF

The histogram for four channel 32-bit pixel buffers.

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

