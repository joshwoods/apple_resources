

- Core Image
- CIFilter
- Color Effect Filters
-  CIColorPosterize 

Protocol

# CIColorPosterize

The properties you use to configure a color posterize filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIColorPosterize
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var levels: Float

The number of brightness levels to use for each color component.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func colorPosterize() -> any CIFilter &amp; CIColorPosterize

Flattens an image’s colors.

