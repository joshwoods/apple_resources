

- Core Image
- CIFilter
- Halftone Effect Filters
-  CIHatchedScreen 

Protocol

# CIHatchedScreen

The properties you use to configure a hatched screen filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIHatchedScreen
```

## Topics

### Instance Properties

var angle: Float

The angle of the pattern.

**Required**

var center: CGPoint

The x and y position to use as the center of the hatched screen pattern.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var sharpness: Float

The amount of sharpening to apply.

**Required**

var width: Float

The distance between lines in the pattern.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func hatchedScreen() -> any CIFilter &amp; CIHatchedScreen

Creates a monochrome image with a series of lines to add detail.

