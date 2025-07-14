

- Core Image
- CIFilter
- Color Adjustment Filters
-  CIWhitePointAdjust 

Protocol

# CIWhitePointAdjust

The properties you use to configure a white-point adjust filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIWhitePointAdjust
```

## Topics

### Instance Properties

var color: CIColor

A color to use as the white point.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func whitePointAdjust() -> any CIFilter &amp; CIWhitePointAdjust

Adjusts the image’s white-point.

