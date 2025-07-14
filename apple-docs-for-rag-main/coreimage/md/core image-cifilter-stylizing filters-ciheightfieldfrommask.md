

- Core Image
- CIFilter
- Stylizing Filters
-  CIHeightFieldFromMask 

Protocol

# CIHeightFieldFromMask

The properties you use to configure a height-field-from-mask filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIHeightFieldFromMask
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var radius: Float

The length of the height-field transition.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func heightFieldFromMask() -> any CIFilter &amp; CIHeightFieldFromMask

Creates a realistic shaded height-field image.

