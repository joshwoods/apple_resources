

- Core Image
- CIFilter
- Color Effect Filters
-  CIColorCurves 

Protocol

# CIColorCurves

The properties you use to configure a color curves filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIColorCurves
```

## Topics

### Instance Properties

var colorSpace: CGColorSpace?

The working color space.

**Required**

var curvesData: Data

Color values that determine the color curves transform.

**Required**

var curvesDomain: CIVector

A two-element vector that defines the minimum and maximum values of the curve data.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func colorCurves() -> any CIFilter &amp; CIColorCurves

Adjusts an image’s color curves.

