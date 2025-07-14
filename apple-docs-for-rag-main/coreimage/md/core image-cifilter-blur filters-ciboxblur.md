

- Core Image
- CIFilter
- Blur Filters
-  CIBoxBlur 

Protocol

# CIBoxBlur

The properties you use to configure a box blur filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIBoxBlur
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var radius: Float

The radius of the blur, in pixels.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func boxBlur() -> any CIFilter &amp; CIBoxBlur

Applies a square-shaped blur to an area of an image.

