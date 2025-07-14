

- Core Image
- CIFilter
- Color Effect Filters
-  CIColorInvert 

Protocol

# CIColorInvert

The properties you use to configure a color invert filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIColorInvert
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

class func colorInvert() -> any CIFilter &amp; CIColorInvert

Inverts an image’s colors.

