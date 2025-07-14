

- Core Image
- CIFilter
- Color Adjustment Filters
-  CIColorMatrix 

Protocol

# CIColorMatrix

The properties you use to configure a color matrix filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIColorMatrix
```

## Topics

### Instance Properties

var aVector: CIVector

The amount of alpha to multiply the source color values by.

**Required**

var bVector: CIVector

The amount of blue to multiply the source color values by.

**Required**

var gVector: CIVector

The amount of green to multiply the source color values by.

**Required**

var rVector: CIVector

The amount of red to multiply the source color values by.

**Required**

var biasVector: CIVector

A vector that’s added to each color component.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func colorMatrix() -> any CIFilter &amp; CIColorMatrix

Alters the colors in an image based on vectors provided.

