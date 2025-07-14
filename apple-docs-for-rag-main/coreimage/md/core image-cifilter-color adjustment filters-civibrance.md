

- Core Image
- CIFilter
- Color Adjustment Filters
-  CIVibrance 

Protocol

# CIVibrance

The properties you use to configure a vibrance filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIVibrance
```

## Topics

### Instance Properties

var amount: Float

The amount to adjust the saturation by.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func vibrance() -> any CIFilter &amp; CIVibrance

Adjusts an image’s vibrancy.

