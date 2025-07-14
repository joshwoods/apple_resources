

- Metal Performance Shaders
- Image Filters
-  MPSImageGaussianBlur 

Class

# MPSImageGaussianBlur

A filter that convolves an image with a Gaussian blur of a given sigma in both the x and y directions.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageGaussianBlur : MPSUnaryImageKernel
```

## Overview

Note

The Gaussian blur utilizes a very fast algorithm that typically runs at approximately half the speed of copy speeds. Notably, it is faster than either the tent or box blur except perhaps for very large filter windows. Mathematically, it is an approximate Gaussian. Some non-Gaussian behavior may be detectable with advanced analytical methods such as FFT.

If an analytically clean Gaussian filter is required, use the MPSImageConvolution filter instead with an appropriate set of weights. The MPSImageGaussianBlur filter is intended to be suitable for all common image processing needs demanding ~10 bits of precision or less.

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

### Methods

init(device: any MTLDevice, sigma: Float)

Initializes a Gaussian blur filter.

### Properties

var sigma: Float

The sigma value with which the filter was created.

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

