

- Metal Performance Shaders
- Image Filters
-  MPSImageAreaMax 

Class

# MPSImageAreaMax

A filter that finds the maximum pixel value in a rectangular region centered around each pixel in the source image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageAreaMax : MPSUnaryImageKernel
```

## Overview

If there are multiple channels in the source image, each channel is processed independently. The edgeMode property value is assumed to always be MPSImageEdgeMode.clamp for this filter.

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

### Methods

init(device: any MTLDevice, kernelWidth: Int, kernelHeight: Int)

Initializes the kernel with a specified width and height.

### Properties

var kernelHeight: Int

The height of the filter window. Must be an odd number.

var kernelWidth: Int

The width of the filter window. Must be an odd number.

## Relationships

### Inherits From

- MPSUnaryImageKernel

## See Also

### Morphological Image Filters

class MPSImageDilate

A filter that finds the maximum pixel value in a rectangular region by applying a dilation function.

class MPSImageAreaMin

A filter that finds the minimum pixel value in a rectangular region centered around each pixel in the source image.

class MPSImageErode

A filter that finds the minimum pixel value in a rectangular region by applying an erosion function.

