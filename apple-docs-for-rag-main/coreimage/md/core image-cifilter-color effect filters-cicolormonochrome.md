

- Core Image
- CIFilter
- Color Effect Filters
-  CIColorMonochrome 

Protocol

# CIColorMonochrome

The properties you use to configure a color monochrome filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIColorMonochrome
```

## Topics

### Instance Properties

var color: CIColor

The monochrome color to apply to the image.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var intensity: Float

The intensity of the monochrome effect.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func colorMonochrome() -> any CIFilter &amp; CIColorMonochrome

Adjusts an image’s colors to shades of a single color.

