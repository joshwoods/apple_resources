

- Core Image
- CIFilter
- Color Effect Filters
-  CIPalettize 

Protocol

# CIPalettize

The properties you use to configure a palettize filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIPalettize
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var paletteImage: CIImage?

The input color palette, obtained by using a k-means clustering filter.

**Required**

var perceptual: Bool

A Boolean value that specifies whether the filter applies the color palette in a perceptual color space.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func palettize() -> any CIFilter &amp; CIPalettize

Replaces colors with colors from a palette image.

