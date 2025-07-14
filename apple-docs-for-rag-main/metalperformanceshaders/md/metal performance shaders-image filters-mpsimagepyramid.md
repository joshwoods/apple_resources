

- Metal Performance Shaders
- Image Filters
-  MPSImagePyramid 

Class

# MPSImagePyramid

A base class for creating different kinds of pyramid images.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
class MPSImagePyramid : MPSUnaryImageKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

### Methods

init(device: any MTLDevice)

Initializes a downwards 5-tap image pyramid with the default filter kernel and device.

init(device: any MTLDevice, centerWeight: Float)

Initialize a downwards 5-tap image pyramid with a central weight parameter and device.

init(device: any MTLDevice, kernelWidth: Int, kernelHeight: Int, weights: UnsafePointer&lt;Float>)

Initialize a downwards n-tap image pyramid with a custom filter kernel and device.

### Properties

var kernelWidth: Int

The width of the filter window. Must be an odd number.

var kernelHeight: Int

The height of the filter window. Must be an odd number.

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

class MPSImageLaplacian

An optimized Laplacian filter, provided for ease of use.

class MPSImageLaplacianPyramid

A filter that convolves an image with a Laplacian filter.

class MPSImageLaplacianPyramidAdd

A filter that convolves an image with an additive Laplacian pyramid.

class MPSImageLaplacianPyramidSubtract

A filter that convolves an image with a subtractive Laplacian pyramid.

