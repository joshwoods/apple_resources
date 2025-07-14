

- Metal Performance Shaders
- Image Filters
-  MPSImageThresholdToZeroInverse 

Class

# MPSImageThresholdToZeroInverse

A filter that returns 0 for each pixel with a value greater than a specified threshold or the original value otherwise.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageThresholdToZeroInverse : MPSUnaryImageKernel
```

## Overview

An `MPSImageThresholdToZeroInverse` filter converts a single channel image to a binary image. If the input image is not a single channel image, the function first converts the input image into a single channel luminance image using the linear gray color transform, and then it applies the threshold.

Listing 1 shows the threshold to zero inverse function.

destinationPixelValue = sourcePixelValue > thresholdValue ? 0 : sourcePixelValue

Listing 1 Threshold to zero inverse function

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

### New Methods

init(device: any MTLDevice, thresholdValue: Float, linearGrayColorTransform: UnsafePointer&lt;Float>?)

Initializes the kernel.

### Properties

var thresholdValue: Float

The threshold value used to initialize the threshold filter.

var transform: UnsafePointer&lt;Float>

The color transform used to initialize the threshold filter.

## Relationships

### Inherits From

- MPSUnaryImageKernel

## See Also

### Image Threshold Filters

class MPSImageThresholdBinary

A filter that returns a specified value for each pixel with a value greater than a specified threshold or 0 otherwise.

class MPSImageThresholdBinaryInverse

A filter that returns 0 for each pixel with a value greater than a specified threshold or a specified value otherwise.

class MPSImageThresholdToZero

A filter that returns the original value for each pixel with a value greater than a specified threshold or 0 otherwise.

class MPSImageThresholdTruncate

A filter that clamps the return value to an upper specified value.

