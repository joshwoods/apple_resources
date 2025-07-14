

- Metal Performance Shaders
- Image Filters
-  MPSImageAreaMin 

Class

# MPSImageAreaMin

A filter that finds the minimum pixel value in a rectangular region centered around each pixel in the source image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageAreaMin : MPSImageAreaMax
```

## Overview

An `MPSImageAreaMin` filter has the same methods and properties as the MPSImageAreaMax class.

If there are multiple channels in the source image, each channel is processed independently. The edgeMode property value is assumed to always be MPSImageEdgeMode.clamp for this filter.

## Relationships

### Inherits From

- MPSImageAreaMax

## See Also

### Morphological Image Filters

class MPSImageAreaMax

A filter that finds the maximum pixel value in a rectangular region centered around each pixel in the source image.

class MPSImageDilate

A filter that finds the maximum pixel value in a rectangular region by applying a dilation function.

class MPSImageErode

A filter that finds the minimum pixel value in a rectangular region by applying an erosion function.

