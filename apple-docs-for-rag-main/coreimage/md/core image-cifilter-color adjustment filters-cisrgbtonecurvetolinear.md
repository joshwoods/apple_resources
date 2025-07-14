

- Core Image
- CIFilter
- Color Adjustment Filters
-  CISRGBToneCurveToLinear 

Protocol

# CISRGBToneCurveToLinear

The properties you use to configure an sRGB-to-linear filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CISRGBToneCurveToLinear
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func sRGBToneCurveToLinear() -> any CIFilter &amp; CISRGBToneCurveToLinear

Converts the colors in an image from sRGB to linear.

