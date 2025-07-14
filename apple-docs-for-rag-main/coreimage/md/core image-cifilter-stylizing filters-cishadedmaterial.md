

- Core Image
- CIFilter
- Stylizing Filters
-  CIShadedMaterial 

Protocol

# CIShadedMaterial

The properties you use to configure a shaded material filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIShadedMaterial
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var scale: Float

The scale of the effect.

**Required**

var shadingImage: CIImage?

The image to use as the height field.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func shadedMaterial() -> any CIFilter &amp; CIShadedMaterial

Creates a shaded image from a height-field image.

