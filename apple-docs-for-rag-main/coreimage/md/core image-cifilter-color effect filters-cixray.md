

- Core Image
- CIFilter
- Color Effect Filters
-  CIXRay 

Protocol

# CIXRay

The properties you use to configure an X-ray filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIXRay
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

class func xRay() -> any CIFilter &amp; CIXRay

Alters an image to make it look like an X-ray image.

