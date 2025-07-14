

- Core Image
- CIFilter
- Color Adjustment Filters
-  CILinearToSRGBToneCurve 

Protocol

# CILinearToSRGBToneCurve

The properties you use to configure a linear-to-sRGB filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CILinearToSRGBToneCurve
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

class func linearToSRGBToneCurve() -> any CIFilter &amp; CILinearToSRGBToneCurve

Alters an image’s color intensity.

