

- Metal Performance Shaders
-  MPSImageCanny 

Class

# MPSImageCanny

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MPSImageCanny : MPSUnaryImageKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice)

init(device: any MTLDevice, linearToGrayScaleTransform: UnsafePointer&lt;Float>, sigma: Float)

### Instance Properties

var colorTransform: UnsafePointer&lt;Float>

var highThreshold: Float

var lowThreshold: Float

var sigma: Float

var useFastMode: Bool

## Relationships

### Inherits From

- MPSUnaryImageKernel

