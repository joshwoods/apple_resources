

- Core Image
- CIFilter
- Convolution Filters
-  CIConvolution 

Protocol

# CIConvolution

The properties you use to configure a convolution filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIConvolution
```

## Topics

### Instance Properties

var bias: Float

A value that’s added to each output pixel.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var weights: CIVector

The convolution kernel.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func convolution3X3() -> any CIFilter &amp; CIConvolution

Applies a convolution 3 x 3 filter to the `RGBA` components of an image.

class func convolution5X5() -> any CIFilter &amp; CIConvolution

Applies a convolution 5 x 5 filter to the `RGBA` components image.

class func convolution7X7() -> any CIFilter &amp; CIConvolution

Applies a convolution 7 x 7 filter to the `RGBA` color components of an image.

class func convolution9Horizontal() -> any CIFilter &amp; CIConvolution

Applies a convolution-9 horizontal filter to the `RGBA` components of an image.

class func convolution9Vertical() -> any CIFilter &amp; CIConvolution

Applies a convolution-9 vertical filter to the `RGBA` components of an image.

