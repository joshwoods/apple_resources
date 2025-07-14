

- Metal Performance Shaders
- Image Filters
-  MPSImageTent 

Class

# MPSImageTent

A filter that convolves an image with a tent filter.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageTent : MPSImageBox
```

## Overview

The kernel elements of the filter form a tent shape with increasing sides, for example:

Like a box filter, this arrangement allows for much faster algorithms, especially for larger blur radii but with a more pleasing appearance.

The tent blur is a separable filter and the Metal Performance Shaders framework will act accordingly to give the best performance for multi-dimensional blurs.

Note

The box filter, while fast, may yield square-ish looking blur effects. However, multiple passes of the box filter tend to smooth out with each additional pass. For example, two 3-wide box blurs produces the same effective convolution as a 5-wide tent blur.

In effect, addition passes tend to approximate a Gaussian line shape.

## Relationships

### Inherits From

- MPSImageBox

## See Also

### Convolution Image Filters

class MPSImageConvolution

A filter that convolves an image with a given kernel of odd width and height.

class MPSImageMedian

A filter that applies a median filter in a square region centered around each pixel in the source image.

class MPSImageBox

A filter that convolves an image with a given kernel of odd width and height.

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

