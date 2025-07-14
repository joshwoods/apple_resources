

- Core Image
- CIFilter
- Color Adjustment Filters
-  CITemperatureAndTint 

Protocol

# CITemperatureAndTint

The properties you use to configure a temperature and tint filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CITemperatureAndTint
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var neutral: CIVector

A vector containing the source white point defined by color temperature and tint.

**Required**

var targetNeutral: CIVector

A vector containing the desired white point defined by color temperature and tint.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func temperatureAndTint() -> any CIFilter &amp; CITemperatureAndTint

Alters an image’s temperature and tint.

