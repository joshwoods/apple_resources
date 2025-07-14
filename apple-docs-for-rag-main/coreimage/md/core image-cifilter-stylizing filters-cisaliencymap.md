

- Core Image
- CIFilter
- Stylizing Filters
-  CISaliencyMap 

Protocol

# CISaliencyMap

The properties you use to configure a saliency map filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CISaliencyMap
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

class func saliencyMap() -> any CIFilter &amp; CISaliencyMap

Creates a saliency map from an image.

