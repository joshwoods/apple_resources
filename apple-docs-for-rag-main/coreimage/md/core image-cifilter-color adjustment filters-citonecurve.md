

- Core Image
- CIFilter
- Color Adjustment Filters
-  CIToneCurve 

Protocol

# CIToneCurve

The properties you use to configure a tone curve filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIToneCurve
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var point0: CGPoint

A vector containing the position of the first point of the tone curve.

**Required**

var point1: CGPoint

A vector containing the position of the second point of the tone curve.

**Required**

var point2: CGPoint

A vector containing the position of the third point of the tone curve.

**Required**

var point3: CGPoint

A vector containing the position of the fourth point of the tone curve.

**Required**

var point4: CGPoint

A vector containing the position of the fifth point of the tone curve.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func toneCurve() -> any CIFilter &amp; CIToneCurve

Alters an image’s tone curve according to a series of data points.

