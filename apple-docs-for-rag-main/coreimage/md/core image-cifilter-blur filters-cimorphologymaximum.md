

- Core Image
- CIFilter
- Blur Filters
-  CIMorphologyMaximum 

Protocol

# CIMorphologyMaximum

The properties you use to configure a morphology maximum filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIMorphologyMaximum
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var radius: Float

The radius of the circular morphological structuring element.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func morphologyMaximum() -> any CIFilter &amp; CIMorphologyMaximum

Blurs a circular area by enlarging contrasting pixels.

