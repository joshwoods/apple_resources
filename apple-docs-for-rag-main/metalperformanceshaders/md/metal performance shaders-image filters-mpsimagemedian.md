

- Metal Performance Shaders
- Image Filters
-  MPSImageMedian 

Class

# MPSImageMedian

A filter that applies a median filter in a square region centered around each pixel in the source image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageMedian : MPSUnaryImageKernel
```

## Overview

An `MPSImageMedian` filter finds the median color value for each channel within a `kernelDiameter * kernelDiameter` window surrounding the pixel of interest. It is a common means of noise reduction and also as a smoothing filter with edge preserving qualities.

Note

The `MPSImageMedian` filter supports only images with 8 or less bits per channel.

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

### Methods

init(device: any MTLDevice, kernelDiameter: Int)

Initializes a filter for a particular kernel size and device.

class func maxKernelDiameter() -> Int

Queries the maximum diameter, in pixels, of the filter window supported by the median filter.

class func minKernelDiameter() -> Int

Queries the minimum diameter, in pixels, of the filter window supported by the median filter.

### Properties

var kernelDiameter: Int

The diameter, in pixels, of the filter window.

## Relationships

### Inherits From

- MPSUnaryImageKernel

## See Also

### Convolution Image Filters

class MPSImageConvolution

A filter that convolves an image with a given kernel of odd width and height.

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

