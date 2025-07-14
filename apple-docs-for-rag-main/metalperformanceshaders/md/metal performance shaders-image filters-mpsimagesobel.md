

- Metal Performance Shaders
- Image Filters
-  MPSImageSobel 

Class

# MPSImageSobel

A filter that convolves an image with the Sobel operator.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageSobel : MPSUnaryImageKernel
```

## Overview

When the color model (e.g. RGB, two-channel, grayscale, etc.) of the source and destination textures match, the filter is applied to each color channel separately. If the destination is single-channel (i.e. monochrome) but the source is multi-channel, the pixel values are converted to grayscale before applying the Sobel operator by using the linear gray color transform vector `v `shown in the code listing below.

Luminance = v[0] * pixel.x + v[1] * pixel.y + v[2] * pixel.z

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

### Methods

init(device: any MTLDevice)

Initializes a Sobel filter on a given device using the default color transform.

init(device: any MTLDevice, linearGrayColorTransform: UnsafePointer&lt;Float>)

Initializes a Sobel filter on a given device using a specific color transform.

### Properties

var colorTransform: UnsafePointer&lt;Float>

The color transform used to initialize the Sobel filter.

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

