

- Core Image
- CIFilter
- Halftone Effect Filters
-  CICircularScreen 

Protocol

# CICircularScreen

The properties you use to configure a circular screen filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CICircularScreen
```

## Topics

### Instance Properties

var center: CGPoint

The x and y position to use as the center of the circular screen pattern.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var sharpness: Float

The sharpness of the circles.

**Required**

var width: Float

The distance between each circle in the pattern.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func circularScreen() -> any CIFilter &amp; CICircularScreen

Adds a circular overlay to an image.

