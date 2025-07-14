

- Core Image
- CIFilter
- Halftone Effect Filters
-  CIDotScreen 

Protocol

# CIDotScreen

The properties you use to configure a dot screen filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIDotScreen
```

## Topics

### Instance Properties

var angle: Float

The angle of the pattern.

**Required**

var center: CGPoint

The x and y position to use as the center of the dot screen pattern.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var sharpness: Float

The sharpness of the pattern.

**Required**

var width: Float

The distance between dots in the pattern.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func dotScreen() -> any CIFilter &amp; CIDotScreen

Creates a monochrome image with a series of dots to add detail.

