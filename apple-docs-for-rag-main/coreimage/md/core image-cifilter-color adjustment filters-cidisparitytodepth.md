

- Core Image
- CIFilter
- Color Adjustment Filters
-  CIDisparityToDepth 

Protocol

# CIDisparityToDepth

The properties you use to configure a disparity-to-depth filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIDisparityToDepth
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

class func disparityToDepth() -> any CIFilter &amp; CIDisparityToDepth

Creates depth data from an image containing disparity data.

