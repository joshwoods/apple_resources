

- Core Image
- CIFilter
- Stylizing Filters
-  CIBlendWithMask 

Protocol

# CIBlendWithMask

The properties you use to configure a blend with mask filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIBlendWithMask
```

## Topics

### Instance Properties

var backgroundImage: CIImage?

The image to use as a background image.

**Required**

var inputImage: CIImage?

The image to use as a foreground image.

**Required**

var maskImage: CIImage?

A grayscale mask that defines the blend.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func blendWithMask() -> any CIFilter &amp; CIBlendWithMask

Blends two images by using a mask image.

