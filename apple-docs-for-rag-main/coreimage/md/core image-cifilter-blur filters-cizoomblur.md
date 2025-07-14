

- Core Image
- CIFilter
- Blur Filters
-  CIZoomBlur 

Protocol

# CIZoomBlur

The properties you use to configure a zoom blur filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIZoomBlur
```

## Topics

### Instance Properties

var amount: Float

The zoom-in amount.

**Required**

var center: CGPoint

The center of the effect, as x and y coordinates.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func zoomBlur() -> any CIFilter &amp; CIZoomBlur

Creates a zoom blur centered around a single point on the image.

