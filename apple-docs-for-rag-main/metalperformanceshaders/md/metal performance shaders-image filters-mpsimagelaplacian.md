

- Metal Performance Shaders
- Image Filters
-  MPSImageLaplacian 

Class

# MPSImageLaplacian

An optimized Laplacian filter, provided for ease of use.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
class MPSImageLaplacian : MPSUnaryImageKernel
```

## Overview

This filter uses an optimized convolution filter with a 3x3 kernel with the following weights:

Note

The optimized convolution filter used by the `MPSImageLaplacian` class could also be created by initializing an MPSImageConvolution object with `kernelWidth=3`, `kernelHeight=3`, and the weights specified above.

## Topics

### Properties

var bias: Float

The value added to a convolved pixel before it is converted back to its intended storage format.

## Relationships

### Inherits From

- MPSUnaryImageKernel

## See Also

### Convolution Image Filters

class MPSImageConvolution

A filter that convolves an image with a given kernel of odd width and height.

class MPSImageMedian

A filter that applies a median filter in a square region centered around each pixel in the source image.

class MPSImageBox

A filter that convolves an image with a given kernel of odd width and height.

class MPSImageTent

A filter that convolves an image with a tent filter.

class MPSImageGaussianBlur

A filter that convolves an image with a Gaussian blur of a given sigma in both the x and y directions.

class MPSImageGaussianPyramid

A filter that convolves an image with a Gaussian pyramid.

class MPSImageSobel

A filter that convolves an image with the Sobel operator.

class MPSImageLaplacianPyramid

A filter that convolves an image with a Laplacian filter.

class MPSImageLaplacianPyramidAdd

A filter that convolves an image with an additive Laplacian pyramid.

class MPSImageLaplacianPyramidSubtract

A filter that convolves an image with a subtractive Laplacian pyramid.

class MPSImagePyramid

A base class for creating different kinds of pyramid images.

