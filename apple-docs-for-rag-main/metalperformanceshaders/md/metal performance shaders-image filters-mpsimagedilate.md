

- Metal Performance Shaders
- Image Filters
-  MPSImageDilate 

Class

# MPSImageDilate

A filter that finds the maximum pixel value in a rectangular region by applying a dilation function.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageDilate : MPSUnaryImageKernel
```

## Overview

An `MPSImageDilate` filter behaves like the MPSImageAreaMax filter, except Metal calculates the intensity at each position relative to a different value before determining which is the maximum pixel value, allowing for shaped, nonrectangular morphological probes.

The code example below shows pseudocode for the calculation that returns each pixel value:

for each pixel in the filter window
    value = pixel[filterY][filterX] - filter[filterY*filter_width+filterX]
    if( value > bestValue ){
        result = value
        bestValue = value
    }

A filter that contains all zeros is identical to an MPSImageAreaMax filter. Metal handles the center filter element as `0` to avoid causing a general darkening of the image, and it handles the edgeMode property as MPSImageEdgeMode.clamp for this filter.

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

### Methods

init(device: any MTLDevice, kernelWidth: Int, kernelHeight: Int, values: UnsafePointer&lt;Float>)

Initializes the kernel with a specified width, height, and weight values.

### Properties

var kernelHeight: Int

The height of the filter window. which must be an odd number.

var kernelWidth: Int

The width of the filter window which must be an odd number.

## Relationships

### Inherits From

- MPSUnaryImageKernel

## See Also

### Morphological Image Filters

class MPSImageAreaMax

A filter that finds the maximum pixel value in a rectangular region centered around each pixel in the source image.

class MPSImageAreaMin

A filter that finds the minimum pixel value in a rectangular region centered around each pixel in the source image.

class MPSImageErode

A filter that finds the minimum pixel value in a rectangular region by applying an erosion function.

