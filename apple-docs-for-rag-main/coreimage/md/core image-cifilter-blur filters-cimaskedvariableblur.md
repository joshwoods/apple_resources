

- Core Image
- CIFilter
- Blur Filters
-  CIMaskedVariableBlur 

Protocol

# CIMaskedVariableBlur

The properties you use to configure a masked variable blur filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIMaskedVariableBlur
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var mask: CIImage?

A grayscale mask that defines the blur amount.

**Required**

var radius: Float

The distance from the center of the effect.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func maskedVariableBlur() -> any CIFilter &amp; CIMaskedVariableBlur

Blurs a specified portion of an image.

