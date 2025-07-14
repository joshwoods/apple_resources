

- Core Image
- CIFilter
- Color Adjustment Filters
-  CIExposureAdjust 

Protocol

# CIExposureAdjust

The properties you use to configure an exposure adjust filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIExposureAdjust
```

## Topics

### Instance Properties

var ev: Float

The amount to adjust the exposure of the image by.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func exposureAdjust() -> any CIFilter &amp; CIExposureAdjust

Adjusts an image’s exposure.

