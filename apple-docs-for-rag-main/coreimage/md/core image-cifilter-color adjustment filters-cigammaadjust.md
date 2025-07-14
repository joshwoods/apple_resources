

- Core Image
- CIFilter
- Color Adjustment Filters
-  CIGammaAdjust 

Protocol

# CIGammaAdjust

The properties you use to configure a gamma adjust filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIGammaAdjust
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var power: Float

A gamma value to use to correct image brightness.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func gammaAdjust() -> any CIFilter &amp; CIGammaAdjust

Alters an image’s transition between black and white.

