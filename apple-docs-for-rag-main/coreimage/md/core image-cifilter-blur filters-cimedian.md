

- Core Image
- CIFilter
- Blur Filters
-  CIMedian 

Protocol

# CIMedian

The properties you use to configure a median filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIMedian
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

class func median() -> any CIFilter &amp; CIMedian

Calculates the median of an image to refine detail.

