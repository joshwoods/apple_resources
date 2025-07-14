

- Metal Performance Shaders
- Image Filters
-  MPSImageLanczosScale 

Class

# MPSImageLanczosScale

A filter that resizes and changes the aspect ratio of an image using Lanczos resampling.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageLanczosScale : MPSImageScale
```

## Overview

You can use this filter to enlarge or reduce the size of an image, or to change the aspect ratio of an image. The filter uses a Lanczos resampling algorithm, that typically produces better quality for photographs, but is slower than linear sampling that uses GPU texture units. Lanczos downsampling does not require a low pass filter to be applied before it is used. Because the resampling function has negative lobes, Lanczos can result in ringing artifacts near sharp edges, making it less suitable for vector art.

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice)

### Properties

struct MPSScaleTransform

A transform matrix for explicit resampling control with a Lanczos kernel.

## Relationships

### Inherits From

- MPSImageScale

## See Also

### Image Manipulation Filters

class MPSImageConversion

A filter that performs a conversion of color space, alpha, or pixel format.

class MPSImageScale

A filter that resizes and changes the aspect ratio of an image.

class MPSImageBilinearScale

A filter that resizes and changes the aspect ratio of an image using Bilinear resampling.

class MPSImageTranspose

A filter that transposes an image.

