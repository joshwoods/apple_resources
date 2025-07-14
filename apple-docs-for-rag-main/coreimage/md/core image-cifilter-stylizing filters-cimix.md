

- Core Image
- CIFilter
- Stylizing Filters
-  CIMix 

Protocol

# CIMix

The properties you use to configure a mix filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIMix
```

## Topics

### Instance Properties

var amount: Float

The amount of the effect.

**Required**

var backgroundImage: CIImage?

The image to use as a background image.

**Required**

var inputImage: CIImage?

The image to use as a foreground image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func mix() -> any CIFilter &amp; CIMix

Blends two images together.

