

- Accelerate
- vImage
-  vImage Operations 

# vImage Operations

Apply image manipulation operations to vImage buffers.

## Overview

A vImage function name includes the data type of the buffer it operates on. For example, vImageConvolve_Planar8(_:_:_:_:_:_:_:_:_:_:_:) works with 8-bit planar buffers, and vImageConvolve_ARGBFFFF(_:_:_:_:_:_:_:_:_:_:) works with 32-bits-per-channel, four-channel interleaved buffers.

## Topics

### Applying color transforms to images

Transforming with lookup tables

Use lookup tables to apply color transformations to images.

Transforming with polynomials

Use polynomials to apply color transformations to images.

Transforming with matrix multiplication

Use matrix multiplication to apply color transformations to images.

Transforming with a gamma function

Use gamma functions to apply color transformations to images.

Applying a flood fill to an image

Fill connected components of an image with a new color.

### Applying geometric transforms to image buffers

Resampling in vImage

Learn how vImage resamples image data during geometric operations.

Applying affine transformations to images

Translate, rotate, and scale images.

Applying projective transformations to images

Warp images in three dimensions.

Image reflection

Reflect images horizontally and vertically.

Image shearing

Shear images horizontally and vertically.

Image rotation

Rotate images by arbitrary angles or by multiples of 90 degrees.

Image scaling

Scale interlaced and planar images.

Getting the Buffer Size

Calculate the size of the temporary buffer needed by a high-level geometry functions.

### Applying morphological operations to images

Morphology

Dilate and erode images.

### Calculating and modifying an image’s histogram

Histogram

Calculate or manipulate an image’s histogram.

### Clipping data

Clipping data

Clip the pixel values of an image.

### Compositing images using alpha information

Alpha compositing

Composite images together.

### Converting image buffers between formats

Conversion

Convert an image to a different format.

### Convolving images

Convolution

Apply a convolution kernel to an image.

### Extracting channels

Extracting channels

Extract one channel from a four-channel interleaved buffer.

### Filling buffers

Filling buffers

Fill a buffer with a specified color.

### Filtering data prior to decompressing

Decompression Filtering

Filter data prior to decompression.

### Flattening data

Flattening data

Perform an alpha composite of a four-channel image over a solid background color.

### Overwriting channels

Overwriting channels

Overwrite the channels of a buffer.

### Permuting channels

Permuting Channels

Reorder the channels in an image.

### Swapping bytes

Swapping bytes

Byte-swap a buffer.

## See Also

### vImage Operations

Adjusting saturation and applying tone mapping

Convert an RGB image to discrete luminance and chrominance channels, and apply color and contrast treatments.

Blurring an image

Filter an image by convolving it with custom and high-speed kernels.

Adding a bokeh effect to images

Simulate a bokeh effect by applying dilation.

Converting color images to grayscale

Convert an RGB image to grayscale using matrix multiplication.

Building a basic image conversion workflow

Learn the fundamentals of the convert-any-to-any function by converting a CMYK image to an RGB image.

Specifying histograms with vImage

Calculate the histogram of one image, and apply it to a second image.

Enhancing image contrast with histogram manipulation

Enhance and adjust the contrast of an image with histogram equalization and contrast stretching.

Reducing artifacts with custom resampling filters

Implement custom linear interpolation to prevent the ringing effects associated with scaling an image with the default Lanczos algorithm.

Finding the sharpest image in a sequence of captured images

Share image data between vDSP and vImage to compute the sharpest image from a bracketed photo sequence.

