

- Metal Performance Shaders
- Image Filters
-  MPSImageConvolution 

Class

# MPSImageConvolution

A filter that convolves an image with a given kernel of odd width and height.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageConvolution : MPSUnaryImageKernel
```

## Overview

Filter width and height can be either 3, 5, 7 or 9. If there are multiple channels in the source image, each channel is processed independently.

A *separable* convolution filter may perform better when done in two passes. . A convolution filter is separable if the ratio of filter values between all rows is constant over the whole row. For example, this edge detection filter:

Can instead be separated into the product of two vectors, like so:

And consequently can be done as two, one-dimensional convolution passes back to back on the same image. In this way, the number of multiplies (ignoring the fact that we could skip zeros here) is reduced from `3*3=9` to `3+3=6`. There are similar savings for addition. For large filters, the savings can be profound.

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

### Methods

init(device: any MTLDevice, kernelWidth: Int, kernelHeight: Int, weights: UnsafePointer&lt;Float>)

Initializes a convolution filter.

### Properties

var kernelHeight: Int

The height of the filter window. Must be an odd number.

var kernelWidth: Int

The width of the filter window. Must be an odd number.

var bias: Float

The value added to a convolved pixel before it is converted back to its intended storage format.

## Relationships

### Inherits From

- MPSUnaryImageKernel

## See Also

### Convolution Image Filters

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

