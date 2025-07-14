

- Core Image
- CIFilter
- Geometry Adjustment Filters
-  CIPerspectiveTransformWithExtent 

Protocol

# CIPerspectiveTransformWithExtent

The properties you use to configure a perspective transform with extent filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIPerspectiveTransformWithExtent
```

## Topics

### Instance Properties

var extent: CGRect

A rectangle that defines the extent of the effect.

**Required**

## Relationships

### Inherits From

- CIFourCoordinateGeometryFilter

## See Also

### Related Documentation

class func perspectiveTransformWithExtent() -> any CIFilter &amp; CIPerspectiveTransformWithExtent

Alters an image’s geometry to adjust the perspective while applying constraints.

