

- Core Image
- CIFilter
- Stylizing Filters
-  CIPixellate 

Protocol

# CIPixellate

The properties you use to configure a pixellate filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIPixellate
```

## Topics

### Instance Properties

var center: CGPoint

The x and y position to use as the center of the effect.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var scale: Float

A value that determines the size of the squares.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func pixellate() -> any CIFilter &amp; CIPixellate

Enlarges the colors of the pixels to create a blurred effect.

