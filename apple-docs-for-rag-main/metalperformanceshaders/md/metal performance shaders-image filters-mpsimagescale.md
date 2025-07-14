

- Metal Performance Shaders
- Image Filters
-  MPSImageScale 

Class

# MPSImageScale

A filter that resizes and changes the aspect ratio of an image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSImageScale : MPSUnaryImageKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice)

### Instance Properties

var scaleTransform: UnsafePointer&lt;MPSScaleTransform>?

## Relationships

### Inherits From

- MPSUnaryImageKernel

## See Also

### Image Manipulation Filters

class MPSImageConversion

A filter that performs a conversion of color space, alpha, or pixel format.

class MPSImageLanczosScale

A filter that resizes and changes the aspect ratio of an image using Lanczos resampling.

class MPSImageBilinearScale

A filter that resizes and changes the aspect ratio of an image using Bilinear resampling.

class MPSImageTranspose

A filter that transposes an image.

