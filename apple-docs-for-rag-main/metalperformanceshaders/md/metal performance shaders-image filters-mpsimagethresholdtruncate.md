

- Metal Performance Shaders
- Image Filters
-  MPSImageThresholdTruncate 

Class

# MPSImageThresholdTruncate

A filter that clamps the return value to an upper specified value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageThresholdTruncate : MPSUnaryImageKernel
```

## Overview

An `MPSImageThresholdTruncate` filter converts a single channel image to a binary image. If the input image is not a single channel image, the function first converts the input image into a single channel luminance image using the linear gray color transform, and then it applies the threshold.

Listing 1 shows the threshold truncate function.

destinationPixelValue = sourcePixelValue > thresholdValue ? thresholdValue : sourcePixelValue

Listing 1 Threshold truncate function

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

### Methods

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

class MPSImageThresholdToZeroInverse

A filter that returns 0 for each pixel with a value greater than a specified threshold or the original value otherwise.

