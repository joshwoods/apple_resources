

- Metal Performance Shaders
- Image Filters
-  MPSImageErode 

Class

# MPSImageErode

A filter that finds the minimum pixel value in a rectangular region by applying an erosion function.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageErode : MPSImageDilate
```

## Overview

An `MPSImageErode` behaves like the MPSImageAreaMin filter, except that Metal calculates the intensity at each position relative to a different value before determining which is the maximum pixel value, allowing for shaped, nonrectangular morphological probes.

The code example below shows pseudocode for the calculation that returns each pixel value:

for each pixel in the filter window
    value =  pixel[filterY][filterX] + filter[filterY*filter_width+filterX]
    if( value &lt; bestValue ){
        result = value
        bestValue = value
    }

The definition of the `MPSImageErode` filter is different from its `vImage` counterpart (`MPSImageErode_filter_value = 1.0f-vImageErode_filter_value.`). This allows MPSImageDilate and `MPSImageErode` to use the same filter, making open and close operators easier to write.

A filter that contains all zeros is identical to an MPSImageAreaMin filter. Metal handles the center filter element as `0` to avoid causing a general lightening of the image, and it handles the edgeMode property as MPSImageEdgeMode.clamp for this filter.

## Relationships

### Inherits From

- MPSImageDilate

## See Also

### Morphological Image Filters

class MPSImageAreaMax

A filter that finds the maximum pixel value in a rectangular region centered around each pixel in the source image.

class MPSImageDilate

A filter that finds the maximum pixel value in a rectangular region by applying a dilation function.

class MPSImageAreaMin

A filter that finds the minimum pixel value in a rectangular region centered around each pixel in the source image.

