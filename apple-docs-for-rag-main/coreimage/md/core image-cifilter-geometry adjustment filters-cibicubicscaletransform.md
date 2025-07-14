

- Core Image
- CIFilter
- Geometry Adjustment Filters
-  CIBicubicScaleTransform 

Protocol

# CIBicubicScaleTransform

The properties you use to configure a bicubic scale transform filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIBicubicScaleTransform
```

## Topics

### Instance Properties

var aspectRatio: Float

The additional horizontal scaling factor to use on the image.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var parameterB: Float

The value of B to use for the cubic resampling function.

**Required**

var parameterC: Float

The value of C to use for the cubic resampling function.

**Required**

var scale: Float

The scaling factor to use on the image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func bicubicScaleTransform() -> any CIFilter &amp; CIBicubicScaleTransform

Produces a high-quality scaled version of an image.

