

- Metal Performance Shaders
- Image Filters
-  MPSImageIntegral 

Class

# MPSImageIntegral

A filter that calculates the sum of pixels over a specified region in an image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageIntegral : MPSUnaryImageKernel
```

## Overview

The value at each position is the sum of all pixels in a source image rectangle, `sumRect. `Listing 1 shows the pseudocode used to calculate `sumRect`.

sumRect.origin = filter.offset
sumRect.size = dest_position - filter.clipRect.origin

Listing 1 Pseudocode for sumRect

If the channels in the source image are normalized, half-float or floating values, the destination image is recommended to be a 32-bit floating-point image. If the channels in the source image are integer values, it is recommended that an appropriate 32-bit integer image destination format is used.

## Relationships

### Inherits From

- MPSUnaryImageKernel

## See Also

### Image Integral Filters

class MPSImageIntegralOfSquares

A filter that calculates the sum of squared pixels over a specified region in an image.

