

- Metal Performance Shaders
- Image Filters
-  MPSImageBox 

Class

# MPSImageBox

A filter that convolves an image with a given kernel of odd width and height.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageBox : MPSUnaryImageKernel
```

## Overview

The kernel elements all have equal weight, achieving a blur effect (each result is the unweighted average of the surrounding pixels). This allows for much faster algorithms, especially for larger blur radii. The box height and width must be odd numbers.

The box blur is a separable filter and the Metal Performance Shaders framework will act accordingly to give best performance for multi-dimensional blurs.

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

### Methods

init(device: any MTLDevice, kernelWidth: Int, kernelHeight: Int)

Initializes a box filter.

### Properties

var kernelHeight: Int

The height of the filter window. Must be an odd number.

var kernelWidth: Int

The width of the filter window. Must be an odd number.

## Relationships

### Inherits From

- MPSUnaryImageKernel

## See Also

### Convolution Image Filters

class MPSImageConvolution

A filter that convolves an image with a given kernel of odd width and height.

class MPSImageMedian

A filter that applies a median filter in a square region centered around each pixel in the source image.

class MPSImageTent

A filter that convolves an image with a tent filter.

class MPSImageGaussianBlur

A filter that convolves an image with a Gaussian blur of a given sigma in both the x and y directions.

class MPSImageGaussianPyramid

A filter that convolves an image with a Gaussian pyramid.

class MPSImageSobel

A filter that convolves an image with the Sobel operator.

class MPSImageLaplacian

An optimized Laplacian filter, provided for ease of use.

class MPSImageLaplacianPyramid

A filter that convolves an image with a Laplacian filter.

class MPSImageLaplacianPyramidAdd

A filter that convolves an image with an additive Laplacian pyramid.

class MPSImageLaplacianPyramidSubtract

A filter that convolves an image with a subtractive Laplacian pyramid.

class MPSImagePyramid

A base class for creating different kinds of pyramid images.

