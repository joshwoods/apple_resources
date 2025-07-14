

- Core Image
- CIFilter
- Geometry Adjustment Filters
-  CIStraighten 

Protocol

# CIStraighten

The properties you use to configure a straighten filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIStraighten
```

## Topics

### Instance Properties

var angle: Float

The rotation angle, in radians.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func straighten() -> any CIFilter &amp; CIStraighten

Rotates and crops an image.

