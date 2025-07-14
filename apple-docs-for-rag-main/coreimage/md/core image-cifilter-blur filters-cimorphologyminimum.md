

- Core Image
- CIFilter
- Blur Filters
-  CIMorphologyMinimum 

Protocol

# CIMorphologyMinimum

The properties you use to configure a morphology minimum filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIMorphologyMinimum
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

class func morphologyMinimum() -> any CIFilter &amp; CIMorphologyMinimum

Blurs a circular area by reducing contrasting pixels.

