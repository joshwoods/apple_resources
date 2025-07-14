

- Core Image
- CIFilter
- Geometry Adjustment Filters
-  CIPerspectiveCorrection 

Protocol

# CIPerspectiveCorrection

The properties you use to configure a perspective correction filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIPerspectiveCorrection
```

## Topics

### Instance Properties

var crop: Bool

A rectangle that specifies the extent of the corrected image.

**Required**

## Relationships

### Inherits From

- CIFourCoordinateGeometryFilter

## See Also

### Related Documentation

class func perspectiveCorrection() -> any CIFilter &amp; CIPerspectiveCorrection

Transforms an image’s perspective.

